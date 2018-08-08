# Digital-Forensics

Installing Autopsy on Mac
	•	Press Command+Space and type Terminal and press enter/return key.
	•	Run in Terminal app: ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null
and press enter/return key.
	•	Run: brew install autopsy

Done! You can now use autopsy [1]

Problems encountered during installation: None

Mounting a forensic image
Problems encountered during image mounting: 
I tried using the following commands: 
	•	sudo mount -t ntfs-3g -o loop,ro,noexec,offset=32256 imageName.dd
	•	mmls out.dd
But it wasn’t compatible with macOS

Solution:
Run the following command
	•	hdiutil attach -imagekey diskimage-class=CRawDiskImage -nomount imageName.dd
You will get an output indicating the name of the disk being mounted
	•	hdiutil mount DiskNameBeingMounted 
e.g hdiutil mount /dev/disk2

Installing exiftool on Mac
	•	Press Command+Space and type Terminal and press enter/return key.
	•	Run in Terminal app:
$ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null
and press enter/return key.
	•	Run:
brew install exiftool

Done! You can now use exiftool [1]

Problems encountered during installation: None







References
	•	http://macappstore.org/



