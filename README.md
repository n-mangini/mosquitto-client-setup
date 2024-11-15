# Python Client

## Usage

1. **Create a Virtual Environment**  
   Run the following command to create a virtual environment inside [python-client folder](https://github.com/n-mangini/mosquitto-client-setup/tree/main/python-client):
   ```bash
   python3 -m venv venv

2. **Activate the Virtual Environment**  
   Use this command to activate the virtual environment:
   ```bash
   source venv/bin/activate

3. **Install Dependencies**  
   With the virtual environment active, install the required dependency:
   ```bash
   pip install paho-mqtt

4. **Add your own configuration**
   - Create your own config.py using [config.py.template](https://github.com/n-mangini/mosquitto-client-setup/blob/main/python-client/include/config.py.template).
   - Note: use PORT=8883 for secured mode, 1883 for unsecured
     
   ```bash
   cp python-client/include/config.py.template ./python-client/include/config.py && vim python-client/include/config.py
   ```

5. **Add your own certificates**
   Copy the content of your certificate given after running (generate-certificates.sh)[https://github.com/n-mangini/mosquitto-broker-setup/blob/main/mosquitto/certs/generate-ceritificates.sh] in [ca-root-cert.crt](https://github.com/n-mangini/mosquitto-client-setup/blob/main/python-client/include/ca-root-cert.crt.template).

4. **Run the Client Script**  
   Now, you can run the `client.py` script to test the MQTT broker:
   ```bash
   python3 python-client/client.py

## Notes

- Ensure that the MQTT broker is running and accessible before executing the script.
- Use `deactivate` to exit the virtual environment when you're done.

---
