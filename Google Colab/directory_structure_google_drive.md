# To see directory structure in Google Colab

```python
import os

def print_directory_tree(root_path, indent=''):
    # Print current directory name
    print(indent + os.path.basename(root_path) + '/')

    # Get list of directories and files in the current directory
    items = sorted(os.listdir(root_path))

    # Iterate over directories and files
    for item in items:
        item_path = os.path.join(root_path, item)

        # Exclude directories starting with "."
        if os.path.isdir(item_path) and not item.startswith('.'):
            print_directory_tree(item_path, indent + '-')
        elif os.path.isfile(item_path):
            # Print file name
            print(indent + '-' + item)
```