# Image Processing Into Black and White

This repository contains a Python script that uses the `PIL` (Python Imaging Library) and `NumPy` libraries to convert a colorful photo into black and white. Please note that the front end is still under development.

## Prerequisites

Make sure you have the following libraries installed in your Python environment:

- PIL (`pip install Pillow`)
- NumPy (`pip install numpy`)
- Matplotlib (`pip install matplotlib`)

## Usage

1. Import the necessary libraries in your Python script:

```python
from PIL import Image
import numpy as np
import matplotlib.pyplot as plt
```

2. Load the image using PIL:

```python
image = Image.open("path_to_image")
```

3. Convert the PIL image object to a NumPy array:

```python
arr = np.array(image)
```

4. Display the original image:

```python
plt.imshow(arr)
plt.show()
```

5. Convert the image to grayscale:

```python
grey = arr.mean(axis=2)
```

6. Display the grayscale image:

```python
plt.imshow(grey, cmap="gray")
plt.show()
```

## Example

Here's an example of how to use the provided code:

```python
from PIL import Image
import numpy as np
import matplotlib.pyplot as plt

# Load the image
image = Image.open("path_to_image")

# Convert the image to a NumPy array
arr = np.array(image)

# Display the original image
plt.imshow(arr)
plt.show()

# Convert the image to grayscale
grey = arr.mean(axis=2)

# Display the grayscale image
plt.imshow(grey, cmap="gray")
plt.show()
```

## Note

- Make sure to replace `"path_to_image"` with the actual path to your image file.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributions

Contributions to this project are welcome! To contribute, please follow these steps:

1. Fork this repository.
2. Create a new branch: `git checkout -b my-feature-branch`.
3. Make your changes and commit them: `git commit -m "Add new feature"`.
4. Push to the branch: `git push origin my-feature-branch`.
5. Submit a pull request.

If you encounter any issues or have suggestions for improvement, please submit them in the [issue tracker](https://github.com/Jr-Einstein/Image-Processing-Into-Black-and-White/issues).

## Support

If you need any assistance or have any questions, feel free to contact the project maintainers at [amankumar.singh2022@vitbhopal.ac.in(mailto:amankumar.singh2022@vitbhopal.ac.in).

Enjoy image processing with Python!
