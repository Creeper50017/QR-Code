import qrcode

# Get user input
data = input("Введите содержимое QR Кода:")

# Generate QR code
qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=10,
    border=4,
)
qr.add_data(data)
qr.make(fit=True)

# Create an image from the QR Code instance
img = qr.make_image(fill_color="black", back_color="white")

# Save the QR code image
img.save("QR_Code.png")

print("QR Код успешно создан и сохранен в файле QR_Code.png")
