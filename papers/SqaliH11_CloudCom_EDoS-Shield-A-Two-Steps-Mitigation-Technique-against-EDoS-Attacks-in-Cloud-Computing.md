[EDoS-Shield: A Two-Steps Mitigation Technique against EDoS Attacks in Cloud Computing](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6123480&tag=1)
---

-  reading status: finished on 10/15/2014
- bib
```
@INPROCEEDINGS{SqalliA11, 
    author={Sqalli, M.H. and Al-Haidari, F. and Salah, K.}, 
    booktitle={Utility and Cloud Computing (UCC), 2011 Fourth IEEE International Conference on}, 
    title={EDoS-Shield - A Two-Steps Mitigation Technique against EDoS Attacks in Cloud Computing}, 
    year={2011}, 
    pages={49-56}
```

### Summary
In this paper, the authors propose a EDoS mitigating mechanism by verifying whether the requests are from legitimate users or bots. The main components of distinguishing legitimates from bots is achived by CAPTCHA. 


### System Architecture
- The following figures show the system architecure
<div text-align ="center" >
    <img src="../figs/EDoS-Shield.PNG" width="500px"/>
</div>
    - Virtual Firewall(VF): IP white and black list
    - V-Nodes: turing-test, captcha to verify whether it is human or bots

### Weakness
- The proposed mechanism use Turing test to verity legitimate clients from bots 
    - turing test could fail
    - it is unpleasant to users for dealing with the turing test or CAPTCHA
- block IP
    - NAT problem

### Extension
- the system is somewhat similar to our system
    - we both use firewall(load balancer) to redirect clients to authentication node
    - however, we assume some bots may pass the authentication and enter our system. i.e., we are trying to deal with the case when there are insiders in the system.
    
### TODO
- record the related work of *load balancing" of firewall in page 52, these could be evidence of how robust the firewall or loadblancer could be in the cloud
