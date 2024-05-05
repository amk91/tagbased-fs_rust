# Chapters
+ ## [[#Introduction to tag-based file system]]
+ ## [[#Use cases of tag-based file systems]]
+ ## [[#Rust use cases of tag-based file systems]]
+ ## [[#Rust features for tag-based file systems]]
+ ## [[#Citations]]
## Introduction to tag-based file system
A filesystem is a method of organizing, keeping track and accessing files on a storage device. Having a filesystem that governs how data is stored and accessed is necessary to avoid applications from using data in ways that could lead to resource contention, data corruption and data loss. There are different categories of filesystems, to name a few:
- [[#Hierarchical file systems]]
- [[#Flat file systems]]
- [[#Tag-based file systems]]
### Hierarchical file systems
A hierarchical file systems, directories are used to store files and other subdirectories. The file system is organized as a tree structure, with the origin directory as the root of the tree, which is usually saved on a specific location on a storage device.

### Flat file systems
A flat file system is a simplified version of the hierarchical file system where there are no subdirectories and all the files are store in one, root directory.

### Tag-based file systems
Whereas a hierarchical filesystem uses directories which contains information about files and other directories (called subdirectories) organized in a tree structure, a tag-based filesystem utilizes files metadata to organize them on the storage device. The two main type of metadata are the following:
- [[#File type-specific]]
- [[#Tags]]
#### File type-specific
Metadata is extracted directly from the file itself thanks to transducers, which are programmable methods to extract data from specific file types. The transducers use the semantics of the file to build the metadata list used for indexing purposes. Each file type can have its own transducer that will extract specific information from the file. For example, a transducer programmed to retrieve information from an audio file could generated metadata from the following properties: name of the song, name of the album (if applicable), name of the artist, year of release, genre, recording sample rate, etc.

#### Tags
Tags are descriptive strings assigned to each file by the user so that the file can be categorized and searched for later on based on those specific tags. Since the tags are assigned by the user and not derived by the file itself in an automatic way, the tags need to be saved in non-volatile storage. Virtually there should be no limit on how many tags can be assigned to a file.

-----------------------------------
## Use cases of tag-based file systems

## Rust use cases of tag-based file systems

## Rust features for tag-based file systems

## Citations
 1. [Semantic File Systems by Gifford, Jouvelot, Sheldon and O'Toole](https://web.mit.edu/6.826/www/notes/HO13.pdf) 