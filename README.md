import qrcode

# 1. Define the data (URL or Text)
data = "https://github.com/your-username"

# 2. Configure the QR Code settings
qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=10,
    border=4,
)

# 3. Add data to the instance
qr.add_data(data)
qr.make(fit=True)

# 4. Create the image (customize colors here)
img = qr.make_image(fill_color="black", back_color="white")

# 5. Save the image file
img.save("qrcode_project.png")

print("Success! QR code generated as 'qrcode_project.png'")
# AYUSH-new-project-1
New learning python 
