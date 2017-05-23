# OpenAirInterface5G - SDR and Cloud based deployment
This tutorial is intended to setup all the OpenAirInterface5G components using the S1 interface, placing the core components in a cloud based system. The connection between OAI-UE and the OAI-eNB will be carried out by using USRP B210 SDR cards connected using wires and the selected cloud system where cloud components will be deployed will be OpenStack.

## Hardware setup
The proposed deployment has been tested using the hardware showed in the following figure:

![Alt text](/hw_configuration.PNG?raw=true "Optional Title")

The attenuation between UE and eNB should be adjusted between 40 and 60 dB.

## Core components deployment (HSS, MME and SP-GW).
The core components will be deployed in a cloud based system. In this tutorial, we are going to use OpenStack as a virtual machines manager. For this deployment we need three virtual machines, one per OpenAirCN componet with the following configuration:
* Ubuntu 14.04 LTS (32-bits or 64-bits)
* Install git 
  * `sudo apt-get install git`
* Download the latest development branch of OpenAir-cn
  * `git clone https://gitlab.eurecom.fr/oai/openair-cn.git`
  * `git checkout develop`
  * `git fetch && git pull`

### Core Components Network Configuration
Once we have our virtual machines running, we have to configure all the network devices in order to allow the communication between them. We propose the following network configuration (OpenStack):

![Alt text](/oai-cn_network_config.PNG?raw=true "Optional Title")


## Getting Started

Before start building the components, let's start with the hardware 
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you have to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc


