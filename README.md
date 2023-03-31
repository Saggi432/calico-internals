Helpful commands


 *Cluster IP *
sudo iptables -v --numeric --table nat --list KUBE-SERVICES
sudo iptables -v --numeric --table nat --list KUBE-SERVICES | grep -E summary

sudo iptables -v --numeric --table nat --list KUBE-SVC-OIQIZJVJK6E34BR4


* NodePort*

sudo iptables -v --numeric --table nat --list KUBE-SERVICES | grep KUBE-NODEPORTS

sudo iptables -v --numeric --table nat --list KUBE-NODEPORTS


eBPF(Direct Server Return)

sudo tcpdump -nvi any 'tcp port 30180'
