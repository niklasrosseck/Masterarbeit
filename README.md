# Pi Hole Blocklists

This project aims to provide effective blocklists for a variety of applications. To make the blocklists as
effective as possible they are combinations of different publicly available blocklist and self found domains.
The self found domains where found by using Sublist3r. Every used blocklist is linked in the .txt file.
To avoid duplicate entries new entries are first put into the test.txt file and then the check.py normalizes the
entries and only adds new entries to the specified blocklist file.

# Combine Scripts

The scripts for combining blocklists are divided into two scripts. The first script combine_all.py lets you
combine all blocklists together and also combine subdirectories. The standard is to combine all blocklists but by adding directories in the 'exclude_subdirectories' you can customize which directories you want to combine. The second script combine_selected.py lets you choose which blocklists you want to combine regardless of the subdirectory they are in. This is used to create truly individual blocklists. The script first lists all available blocklists and then you can select which blocklists you want to combine.

# Including in Pi Hole

To use these blocklists in your Pi Hole you need to add them to your adlist. You can do this in the
web interface of Pi Hole.
