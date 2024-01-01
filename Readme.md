# The development environment of ns2.35

This work is for the development environment of ns-2.35 on the Mac OS. It also contains some basic works for the malicious study in Ad hoc network simulation. (eg. blackhole-aodv, grayhole-aodv, watchdog(aodv), and Bayesian-watchdog(aodv))


## Base environment
* Host OS: macOS High Sierra version 10.13.4 (may
have issue in other OS)
* Docker base image is [ubuntu:14:04](https://registry.hub.docker.com/u/library/ubuntu/)
* Docker files are based on [docker-ns2](https://github.com/ekiourk/docker-ns2/)
*  Docker develop environment [ns2.35-with-docker](https://hub.docker.com/repository/docker/youhaku/ns2-with-docker/general) can be found in docker hub
* [Miniconda3](https://conda.io/miniconda.html) ( python3.6 and pip3.6 ) is installed along with jupyter notebook.


## Composition
This project includes:

*  How to simulation and project description in [Readthedocs]([https://ns2-simulation.readthedocs.io](https://ns2-simulation.readthedocs.io/))
*  Already being installed source code of [ns2.35](https://www.isi.edu/nsnam/ns/)
*  New protocols including mflood, blackhole-aodv, grayhole-aodv, watchdog(aodv), and Bayesian-watchdog(aodv) 
*  Simulation analyze tools: NSG2.1, APP-tool, py-parser, jupyter notebook


## Tools
* ### tcl generation tool
[NSG2.1](https://sites.google.com/site/pengjungwu/nsg) is developed in Java to make the generation of tcl files easy with GUI

![NSG2.1](https://github.com/amrta-coder/ns2.35-with-docker/blob/main/images/NSG2.1.png)


* ### trace file parser
[APP Tool](https://github.com/WiNG-NITK/APP-Tool) (Automated Post Processing tool) is a ns2 tracefile analyser with GUI

![APP Tool](https://github.com/amrta-coder/ns2.35-with-docker/blob/main/images/APP%20Tools.png)


* ### nam: network animator
[Nam](https://www.isi.edu/nsnam/nam/) is a Tcl/TK-based animation tool for viewing network simulation traces and real-world packet traces.

![Nam](https://github.com/amrta-coder/ns2.35-with-docker/blob/main/images/NAM.png)


* ### jupyter lab
Access to http://localhost:8888 with login password: "jupyter" (or set the password by yourself)

![Jupyterlab](https://github.com/amrta-coder/ns2.35-with-docker/blob/main/images/jupyter.png)

* ### python tools
[ns2 tools](http://www.evanjones.ca/software/ns2tools.html) for simulation preparation and results parser

## Virtualization
To display the GUI (nam / NSG / APP Tool) from docker to macOS you should:
1. Confirm X11 is already installed 
2. Run `xhost + 127.0.0.1` in the host Mac OS in advance.

## Related publications

1. [Historical evidence-based trust management strategy against black hole attacks in MANET](https://ieeexplore.ieee.org/abstract/document/6174693)

```BibTeX
@INPROCEEDINGS{6174693,
  author={Yang, Bo and Yamamoto, Ryo and Tanaka, Yoshiaki},
  booktitle={2012 14th International Conference on Advanced Communication Technology (ICACT)}, 
  title={Historical evidence-based trust management strategy against black hole attacks in MANET}, 
  year={2012},
  volume={},
  number={},
  pages={394-399},
  doi={}}
}
```

2. [Dempster-Shafer evidence theory based trust management strategy against cooperative black hole attacks and gray hole attacks in MANETs](https://ieeexplore.ieee.org/abstract/document/6779177)

```BibTeX
@INPROCEEDINGS{6779177,
  author={Yang, Bo and Yamamoto, Ryo and Tanaka, Yoshiaki},
  booktitle={16th International Conference on Advanced Communication Technology}, 
  title={Dempster-Shafer evidence theory based trust management strategy against cooperative black hole attacks and gray hole attacks in MANETs}, 
  year={2014},
  volume={},
  number={},
  pages={223-232},
  doi={10.1109/ICACT.2014.6779177}}
```
