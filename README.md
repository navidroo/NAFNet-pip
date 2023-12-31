## Project

This project is a version of "NAFNet: Nonlinear Activation Free Network for Image Restoration" that can be installed using pip. It can also be run inside a Docker container. NAFNet was built using BasicSR, and the current project utilizes both NAFNet and BasicSR.


## Docker file

``` latex
FROM "your-base-container"
RUN apt-get update && apt-get install -y git  

RUN git clone https://github.com/navidroo/NAFNet-pip.git   
WORKDIR NAFNet-pip
RUN pip install -r requirements.txt  
RUN pip install -v -e .
```

## Install
```
git clone https://github.com/navidroo/NAFNet-pip.git   
cd NAFNet-pip
pip install -r requirements.txt  
pip install -v -e .
```



## 📜 License and Acknowledgement

This project is released under the [Apache 2.0 license](LICENSE.txt).<br>
More details about **license** and **acknowledgement** are in [LICENSE](LICENSE/README.md).

## 🌏 Citations

If NAFNet-pip helps your research or work, please cite NAFNet-pip.<br>
The following is a BibTeX reference. The BibTeX entry requires the `url` LaTeX package.

### NAFNet-pip
``` latex
@misc{navid2023nafnetpip,
  author =       {Roohani, Navid},
  title =        {{NAFNet-pip}: pip installable NAFNet},
  howpublished = {\url{https://github.com/navidroo/NAFNet-pip.git}},
  year =         {2023}
}
```

### BasicSR
``` latex
@misc{basicsr,
  author =       {Xintao Wang and Liangbin Xie and Ke Yu and Kelvin C.K. Chan and Chen Change Loy and Chao Dong},
  title =        {{BasicSR}: Open Source Image and Video Restoration Toolbox},
  howpublished = {\url{https://github.com/XPixelGroup/BasicSR}},
  year =         {2022}
}
```

> Xintao Wang, Liangbin Xie, Ke Yu, Kelvin C.K. Chan, Chen Change Loy and Chao Dong. BasicSR: Open Source Image and Video Restoration Toolbox. <https://github.com/xinntao/BasicSR>, 2022.

### NAFNet:
``` latex
@article{chen2022simple,
  title={Simple Baselines for Image Restoration},
  author={Chen, Liangyu and Chu, Xiaojie and Zhang, Xiangyu and Sun, Jian},
  journal={arXiv preprint arXiv:2204.04676},
  year={2022}
}
```
