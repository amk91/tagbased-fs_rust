## Chapters
+ #### [[#Introduction to tag-based filesystem]]
	+ [[#Tag-based filesystems]]
	+ [[#File type-specific metadata]]
	+ [[#Tags]]
+ #### [[#Implementations of tag-based filesystems in the real world]]
+ #### [[#Rust implementations of tag-based filesystems]]
+ #### [[#Rust idioms useful during implementation of tag-based filesystems]]
+ #### [[#Citations]]
## Introduction to tag-based filesystem
A filesystem is a method of organizing, keeping track and accessing files on a storage device. Having a filesystem that governs how data is stored and accessed is necessary to avoid applications from using data in ways that could lead to resource contention, data corruption and data loss. There are different categories of filesystems, to name a few:
- Hierarchical filesystem
- Flat file system
- Tag-based filesystem

#### Tag-based filesystems
Whereas a hierarchical filesystem uses directories which contains information about files and other directories (called subdirectories) organized in a tree structure, a tag-based filesystem utilizes files metadata to organize them on the storage device. The two main type of metadata are the following:
- File type-specific
- Tags

#### File type-specific metadata
This kind of metadata is retrieved directly from information available on the file, like date of creation, file extension, etc. Usually for each file type the metadata is retrieved by a transducer. For instance, for source code files, metadata can be the names of the functions exported by the program, or for music files metadata can be the artist name, song name, duration.

#### Tags




-----------------------------------
## Implementations of tag-based filesystems in the real world

## Rust implementations of tag-based filesystems

## Rust idioms useful during implementation of tag-based filesystems

## Citations
- [Semantic File Systems by Gifford // https://web.mit.edu/6.826/www/notes/HO13.pdf](https://web.mit.edu/6.826/www/notes/HO13.pdf)
- 