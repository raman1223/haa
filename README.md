from PIL import Image

# Create a new blank image
image = Image.new('RGB', (500, 500), 'white')

# Draw a dog shape on the image
draw = ImageDraw.Draw(image)
draw.rectangle([(100, 100), (400, 400)], fill='brown')
draw.ellipse([(150, 200), (250, 300)], fill='white')
draw.ellipse([(300, 200), (400, 300)], fill='white')
draw.polygon([(200, 400), (250, 450), (300, 400)], fill='black')

# Save the image
image.save('dog.png')
