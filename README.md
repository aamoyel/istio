# istio w/ kustomize
<div id="top"></div>

<!-- TABLE OF CONTENTS -->
<details open>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>
</br>



<!-- ABOUT THE PROJECT -->
## About The Project
This project allows you to deploy [Istio](https://istio.io/) on Kubernetes with Kustomize binary.

<p align="right">(<a href="#top">back to top</a>)</p>


### Built With
* [Kubernetes](https://kubernetes.io/)
* [Kustomize](https://kustomize.io/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

You need to have :
* An operational Kubernetes cluster
* Kustomize binary
* istioctl binary

### Installation
1. Install Istio with istioctl or other method. With istioctl:
   ```sh
   # Install istio with a specific revision (change 1-14-3 by your version)
   istioctl install -y -r 1-14-3
   ```
2. Clone the repo :
   ```sh
   git clone https://github.com/aamoyel/istio.git && cd istio
   ```
3. Change ingresses files to match your setup
4. Deploy istio addons on your cluster
   ```sh
   kustomize build . | kubectl apply -f -
   ```

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Alan Amoyel - [@AlanAmoyel](https://twitter.com/AlanAmoyel)

Project Link: [https://github.com/aamoyel/istio](https://github.com/aamoyel/istio)

<p align="right">(<a href="#top">back to top</a>)</p>
