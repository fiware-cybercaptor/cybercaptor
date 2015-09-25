CyberCAPTOR
==============

[FIWARE Cyber seCurity Attack graPh moniTORing](https://cybercaptor.readthedocs.org/)

This project is part of FIWARE. For more information, please consult [FIWARE website](http://www.fiware.org/).

CyberCAPTOR is an implementation of the Cyber Security Generic Enabler, the future developments of the [Security Monitoring GE](http://catalogue.fiware.org/enablers/security-monitoring).

# CyberCAPTOR main components

The CyberCAPTOR project is a the main entry-point to deploy CyberCAPTOR-Client, CyberCAPTOR-Server and CyberCAPTOR-P2DS.

CyberCAPTOR is composed of several sub-projects :
  - [CyberCAPTOR-Server](https://github.com/fiware-cybercaptor/cybercaptor-server): the risk assessement server.
  - [CyberCAPTOR-Client](https://github.com/fiware-cybercaptor/cybercaptor-client): the GUI of CyberCAPTOR-Server.
  - [CyberCAPTOR-P2DS](https://github.com/fiware-cybercaptor/cybercaptor-p2ds): the Privacy-Preserving Data Sharing.

The deployment of [CyberCAPTOR-P2DS](https://github.com/fiware-cybercaptor/cybercaptor-p2ds) can be done independently of [CyberCAPTOR-Server](https://github.com/fiware-cybercaptor/cybercaptor-server) and [CyberCAPTOR-Client](https://github.com/fiware-cybercaptor/cybercaptor-client). The main concepts and installation guide of Privacy-Preserving Data Sharing are described in [https://github.com/fiware-cybercaptor/cybercaptor-P2DS/blob/master/p2ds/README.md](https://github.com/fiware-cybercaptor/cybercaptor-P2DS/blob/master/p2ds/README.md).

[CyberCAPTOR-Client](https://github.com/fiware-cybercaptor/cybercaptor-client) is the GUI of [CyberCAPTOR-Server](https://github.com/fiware-cybercaptor/cybercaptor-server). Thus CyberCAPTOR-Client need a CyberCAPTOR-Server to work properly. The main concepts and installation guide of CyberCAPTOR-Client are described in [https://github.com/fiware-cybercaptor/cybercaptor-client/blob/master/README.md](https://github.com/fiware-cybercaptor/cybercaptor-client/blob/master/README.md).

[CyberCAPTOR-Server](https://github.com/fiware-cybercaptor/cybercaptor-server) is a REST API Server, and thus can be deployed independently of CyberCAPTOR-Client. The main concepts and installation guide of CyberCAPTOR-Server are described in [https://github.com/fiware-cybercaptor/cybercaptor-server/blob/master/README.md](https://github.com/fiware-cybercaptor/cybercaptor-server/blob/master/README.md).

# Deploying CyberCAPTOR-Client and CyberCAPTOR-Server in a few seconds with Docker

CyberCAPTOR-Client](https://github.com/fiware-cybercaptor/cybercaptor-client) and [CyberCAPTOR-Server](https://github.com/fiware-cybercaptor/cybercaptor-server) can be deployed in a few seconds, using Docker.

If you have Docker installed, launch the CyberCAPTOR-Server in a Terminal:

```
docker run --rm --name cybercaptor-server -p 8080:8080 fiwarecybercaptor/cybercaptor-server
```

Then, in an other Terminal, launch the CyberCAPTOR-Client:

```
docker run --rm --name cybercaptor-client -p 8000:80 fiwarecybercaptor/cybercaptor-client
```

Then, you can access CyberCAPTOR-Client on [http://localhost:8000](http://localhost:8000).
