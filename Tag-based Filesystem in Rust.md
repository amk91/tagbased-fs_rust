## Chapters
+ #### [[#Introduction to tag-based filesystem]]
	+ [[#Tag-based filesystems]]
	+ [[#File type-specific metadata]]
	+ [[#Tags]]
+ #### [[#Use cases of tag-based filesystems]]
+ #### [[#Rust use cases of tag-based filesystems]]
+ #### [[#Rust features for tag-based filesystems]]
+ #### [[#Citations]]
## Introduction to tag-based filesystem
A filesystem is a method of organizing, keeping track and accessing files on a storage device. Having a filesystem that governs how data is stored and accessed is necessary to avoid applications from using data in ways that could lead to resource contention, data corruption and data loss. There are different categories of filesystems, to name a few:
- Hierarchical filesystem
- Flat file system
- Tag-based filesystem

#### Tag-based filesystems
Whereas a hierarchical filesystem uses directories which contains information about files and other directories (called subdirectories) organized in a tree structure, a tag-based filesystem utilizes files metadata to organize them on the storage device. The two main type of metadata are the following:
- [[#File type-specific]]
- [[#Tags]]

#### File type-specific
Metadata is extracted directly from the file itself thanks to transducers, which are programmable methods to extract data from specific file types. The transducers use the semantics of the file to build the metadata list used for indexing purposes. Each file type can have its own transducer that will extract specific information from the file. For example, a transducer programmed to retrieve information from an audio file could generated metadata from the following properties: name of the song, name of the album (if applicable), name of the artist, year of release, genre, recording sample rate, etc.

#### Tags

-----------------------------------
## Use cases of tag-based filesystems

## Rust use cases of tag-based filesystems

## Rust features for tag-based filesystems

## Citations
 1. [Semantic File Systems by Gifford, Jouvelot, Sheldon and O'Toole](https://web.mit.edu/6.826/www/notes/HO13.pdf) 