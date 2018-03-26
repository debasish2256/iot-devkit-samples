Don't use this branch for development, this is to test the project can be built with the Azure SDK

Build commands:

g++ -I/usr/include/azureiot -I/usr/include/azureiot/inc -I/usr/include -I/usr/include/c++ -O0 -g3 -Wall -c -fmessage-length=0 -std=c++11 -I/usr/include/azureiot -I/usr/include/azureiot/inc --sysroot= -m64 -c -o main.o main.cpp 

-g++ --sysroot= -o Azure_IoT_Hub_with_MQTT main.o -liothub_client -liothub_client_mqtt_transport -laziotsharedutil -lumqtt -lpthread -lcurl -lssl -lcrypto