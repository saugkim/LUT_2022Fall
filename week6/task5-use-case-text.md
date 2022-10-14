
EVENT   	 : Select destination for holiday trip  

ACTOR      : user (signup user or anonymous user)  

CONDITION  : internet to use MAP service and to get geo-coordinates of the selected location
 
SCENARIOS  :

    start view (main view): user selects destination and for this user sees two options
        - user selects the map option       -> user sees map view 
        - user selects the drop-down option -> user sees drop down menu view
        - user can login (possibly sign-up) -> user sees login view
        - signed-up user can save travel history (destination and date) 

    map view with search bar on top: 
        - user navigates map and select location by clicking(tapping) on map
        - user writes name or address using search bar, center of the map will be relocated according to the search result
        - user confirms to return main view or re-select destination       

    drop-down menu view for location selection: 
        - list of all regions(+ sub-category) of Finland in drop down menu to select one
        - user confirms to return to main view or re-select destination

    start view (main view):   
        - user returns and sees destination in updated main view   
  

<br>

EXCEPTIONS :  
   - in case of invalid user input when using search bar, 
    app will notify that location not recognized, user can re-write some place or navigate the map instead
   - in case of offline status, app suggests user to use drop down menu to select destination

<br>

RESULTS    : get name and geo-coordinates of selected location  
   - user sees the final destination in main (start) view
   - app (system) saves the latitude and longitude of destination in memory  
 
