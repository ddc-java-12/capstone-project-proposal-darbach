## Summary

Using your device camera, this augmented reality app overlays route data to give you a better sense of direction
and distance to your destination.

Users may:

* Search for locations to display on a 2-D flat map.
* Search for road travel routes between two locations.
* See their searched locations as markers overlayed onto their smartphone camera view.
* See their searched travel route as a line or arrow overlaid onto the street through their smartphone camera view.
* Save locations for quick access.
* Invite other users to view their location and optionally travel routes in real-time.

## Intended users

* A driver who has an easier time following an augmented reality map.

  > As an Uber driver, I sometimes miss my turns, because I have trouble connecting the turns on my GPS with the cross-streets. Augmented reality makes it simple to understand where I am supposed to turn.

* A geography teacher showing the relative position of locations to students. 

  > My students would have a much better sense of the relative positions of cities, countries, and geographical landmarks, if I could show them the true direction, even through the curvature of the Earth. An augmented reality app would be the perfect to tool to reinforce these ideas.  

## Client component

* **Functionality**
  
  * OAuth with Google sign-in.
  * Display an overlay virtual destination marker and route line on the phone camera.
  * Search for destinations.
  * Get location data from OpenStreetMap.
  * Get route data from OpenRouteService.
  * Invite other users to view real-time location and route.

* **Persistent data**

  * History of searches, matching table on the server for portability between devices.
    
* **Device/external services**
  * [Android Sensor Positions](https://developer.android.com/guide/topics/sensors/sensors_position)
  * [Location services](https://developer.android.com/training/location/)
  * OpenStreetMap:
    * [OpenStreetMap Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API)
    * [OpenRouteService API](https://openrouteservice.org/dev/#/api-docs)
  
    
## Server component

* **Functionality**
  
  * Share real-time location and route with other users.

* **Persistent data**
  
  * User profile.
  * Save favorite locations with a descriptive name.
  * Save a history of searches.
  * Location-share invitations between users
    
* **External services**
  
  * [Google Signin](https://developers.google.com/identity/sign-in/android/)
  * [OpenStreetMap Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API)
  * [OpenRouteService API](https://openrouteservice.org/dev/#/api-docs)
    
## Stretch goals/possible enhancements 

* Add personal notes to markers.

