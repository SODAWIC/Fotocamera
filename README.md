# Fotocamera
Fotocamera
# Code for Image Processing
from PIL import Image, ImageFilter

# Open an image file
image_path = "path/to/your/image.jpg"
image = Image.open(image_path)

# Apply a filter (e.g., Gaussian blur)
blurred_image = image.filter(ImageFilter.GaussianBlur(radius=5))

# Save the processed image
output_path = "path/to/your/output_image.jpg"
blurred_image.save(output_path)

# Display the original and processed images
image.show(title="Original Image")
blurred_image.show(title="Blurred Image")
