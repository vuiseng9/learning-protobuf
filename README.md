# Quick Start on learning protobuf
June'18

Reference: https://developers.google.com/protocol-buffers/docs/pythontutorial

Dependency:
python3, protobuf v2, protobuf-compiler 

Setup
apt-get install protobuf-compiler
pip install protobuf

1. Define a protobuf message definition, the .proto
   see addressbook.proto

2. Compile a message definition
   protoc ./addressbook.py --python_out=./
   you will see a generated addressbook_pb2.py 

3. Go through deploy_addressbook_pb2.ipynb

4. Below is an example of using generated protobuf for an application, execute below script to create entry on addressbook 'myaddressbook.pb'
   python3 write_addressbook.py myaddressbook.pb

5. Retrieve myaddressbook.pb entries
   python3 read_addressbook.py myaddressbook.pb

