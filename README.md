### Python Client

## Instructions

1. **Create a Virtual Environment**  
   Run the following command to create a virtual environment:
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

4. **Run the Client Script**  
   Now, you can run the `client.py` script to test the MQTT broker:
   ```bash
   python3 client.py

## Notes

- Ensure that the MQTT broker is running and accessible before executing the script.
- Use `deactivate` to exit the virtual environment when you're done.

---