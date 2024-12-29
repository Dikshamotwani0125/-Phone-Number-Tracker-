pip install phonenumbers

pip install opencage

pip install folium
A Python-based desktop application built using Tkinter to track phone numbers, fetch their carrier information, and display their approximate geographic location on a map using OpenCage Geocoding API and Folium. This application also provides the ability to open the generated map directly in a web browser.

 Features  
- Phone number tracking: Fetch carrier and country information using phonenumbers.  
- Location Mapping: Display the geographic location on an interactive map generated by Folium.  
- User-friendly Interface: Built with Tkinter for easy interaction.  
- Open the map in a browser: Option to view the generated map directly.  


Requirements  
Make sure you have Python installed. The following libraries are also required:

```bash
pip install phonenumbers opencage folium
```
Setup Instructions  

1. Clone this repository  
   ```bash
   git clone https://github.com/AkarshYash/Location-coordinates-with-The-UI/tree/main
   cd PhoneNumberTracker
   ```

2. Set your OpenCage API Key  
   - Replace the `API_KEY` value in the script with your OpenCage API key.  
     You can get an API key from [OpenCage API](https://opencagedata.com/).  
     ```python
     API_KEY = "your_opencage_api_key"
     ```

3. Add Images (Optional)  
   - Place `logo.png` and `search_icon.png` files in the project directory to ensure the GUI renders properly.  

4. Run the Application  
   ```bash
   python phone_number_tracker.py
   ```

Usage  

1. Enter the phone number (including country code) in the input field.  
   Example: +14155552671  
2. Click the Search button to fetch carrier and country information.  
3. If a valid location is found, a map will be generated.  
4. Click the "View Location" button to open the map in a browser.

 Project Structure  

```bash
PhoneNumberTracker/
│
├── phone_number_tracker.py      # Main Python script  
├── logo.png                     # Logo for the application  
├── search_icon.png              # Search icon for the search button  
├── myLocation.html              # Generated map (created after searching)  
├── README.md                    # This README file  
```

Main Window || Generated Map  
 Dependencies  

- Tkinter: For building the GUI  
- phonenumbers: For parsing and validating phone numbers  
- OpenCage API: For getting location data based on carrier information  
- Folium: For generating interactive maps  
- webbrowser: For opening the generated HTML map in the browser  

Error Handling  

- Invalid Input: If the phone number is not valid, an error message will appear.  
- No Location Found: If the location cannot be fetched, a warning will be shown.  
