AddAutoGenerateToThriftFiles
============================

Quick and nasty app to add &lt;auto-generated /> to the beginning of Thrift files generated in c#.  I resorted to this after not finding any ways of doing this from a batch file.  The idea is that this is called from visual studio pre build after you have generated the thrift files.

Warning this is a 5 minute app and is not  a good example of code, no error checking, no docs, etc.


Usage


CommentAdder.exe &lt; path>

The code then goes through all the subdirectories in the path given.  If it finds a c# file, then it adds  &lt;auto-generated /> to the beginning of the file.
