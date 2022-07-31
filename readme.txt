DayZ Chernarus Svetlojarsk Weapons Showcase / Convention Custom Structure Json File For Console and PC Instructions & Terms Of Use

Spawns a large number of weapons, attachments and ammo inside the warehouse at  14148.66 / 13177.33 which is on the Docks in Svetlojarsk on Chernarus.

Limited Testing on PC Chernarus Local Server DAYZ Version 1.18 July 2021.

Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

If you'd like to edit & customize my Weapons Showcase, simply load "gun-show.dze" into DayZ Editor.

The items included on the tables indicate where the weapon may be found:

Apple = Village.
Cereal = Town.
Police Jacket = Police Stations / Guard Houses.
Green Helmet = Military Areas.
Gas Mask = Contaminated Gas Zones (Permenant).
Flight Helmet = Dynamic Event (usually Helicopters, maybe trains.)
Radar Cap = Trains (probably.)
Binoculars = Hunting Areas.
Firemans Helmet = Fire Stations.
Surgical Hat = Medical Areas.
Netting = Coastal Areas.
Wellington Boots = Farms.

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Stop your server.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "cherno-weapon-showcase.json" from the extracted files to inside the "custom" folder of the mission directory on your server.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/cherno-weapon-showcase.json"]	
	
If you already are calling custom jsons to spawn items or buildings, seperate the files like this:

	"objectSpawnersArr": ["custom/cherno-weapon-showcase.json","custom/anotherfile.json","custom/differentfile.json"]
	
Save your changes & upload if you need to.

Restart your server and the new objects will appear immediatly.

Thanks, Rob.