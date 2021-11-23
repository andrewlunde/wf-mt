# wf-mt
Wells Fargo Multitenant

# Build Command:
```
cd wf-mt ; mkdir -p mta_archives ; mbt build -p=cf -t=mta_archives --mtar=wf-mt.mtar
```

# Deploy Command:
```
cf deploy mta_archives/wf-mt.mtar -f
```

# Subsequent Build+Deploy Commands:
```
mbt build -p=cf -t=mta_archives --mtar=wf-mt.mtar ; cf deploy mta_archives/wf-mt.mtar -f
```

# Undeploy Command:
```
cf undeploy acc -f --delete-services
```
