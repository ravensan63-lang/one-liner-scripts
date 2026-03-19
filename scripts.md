# The list

## Files
# Rename all .jpeg to .jpg in current folder
for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done

# Find and delete all .DS_Store files recursively
find . -name ".DS_Store" -delete

# Show folder sizes, sorted
du -sh */ | sort -rh

## Network
# Find what's using port 3000
lsof -i :3000

# Get your public IP
curl ifconfig.me

## Text
# Count lines in a file
wc -l filename.txt

# Remove duplicate lines from a file
awk '!seen[$0]++' file.txt
