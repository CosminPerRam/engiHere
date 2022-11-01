# EngiHere
This project wants to achieve the ability of a full working minimap in tf2 (server-side).

The ability of having a server-side minimap is not really useful in terms of gameplay, but this is done just as a technical showcase.

## How it works
The Server Plugin sends 'events' to a backend, then said backend proceses those events and then distributes the outcome to a client in a browser.

Example:  
> Server: Player K joined the game.  
Backend: Shows that K is in the server.  
Server: Player K joined BLU.  
Backend: Updates K's team to BLU.  
Server: Player K is now a Heavy.  
Backend: Updates K's class to Heavy.  
Client Q: enters the website and sees that K is a heavy on BLU.
Server: Player K spawned and is now at position X, Y.  
Backend: Updates K's position on the minimap.  
Client Q: sees that K is on the map.

## Technical details
The plugin is in SourceMod and the backend is in Rust (using egui over WASM).  
TODO more details.

## How to do a minimap for a map
TODO
