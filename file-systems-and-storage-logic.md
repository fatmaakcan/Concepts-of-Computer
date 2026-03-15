# FILE SYSTEMS AND STORAGE LOGIC

## 1.Storage Units: HDD vs. SSD

### HDD
-HDD has the mechanical spinning disk and read/write head. 
-It is slower and requires pyhsical motion. 
-Less durable because of being a moving part. 
-It can be noisy and can be warm.

### SSD
-It is consist of flash memory units and completely electronic.
-Extremely fast(direct data access)
-No moving part,it is durable against vibrations.
-Works silently and generates less heat.

## 2.Block Structure
Computers store the information called block parts which is small partition not in one piece.

-Data Management: A file (e.g., a photo) is actually combination of several or alongside blocks.

-Efficiency: When the operating system needs to access data, it does not read the whole disk;it only reads the revelant blocks. It affects reading/writing speed directly.

## 3.File Systems (NTFS - extr - APFS)

*NTFS (New Technology File System)*
Developer: Microsoft
Feature: It is developed in file compression, security permissions and large file support fields. Default system of Windows.

*ext4 (Fourth Extended Filesystem)*
Developer:Linux Community
Feature: Manages the massive amounts of data and common system in Linux based (Ununtu,Android etc.) It is performance and stability focused.

*APFS (Apple File System)*
Developer:Apple (macOS,iOS)
Features: It was optimized for SSDs. It has some modern features such as fast metadata copying, strong encryption and space sharing.