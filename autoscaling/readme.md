kubectl run -it load-test --image=busybox /bin/sh
while true; do wget -q -O- http://hpa-example.default.svc.cluster.local:31001; done
