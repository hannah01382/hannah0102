def encrypt_text(input_text, key):
    encrypted_text = ""
    
    for char in input_text:
        encrypted_char = chr(ord(char) + key)
        encrypted_text += encrypted_char
    
    return encrypted_text

def decrypt_text(input_text, key):
    decrypted_text = ""
    
    for char in input_text:
        decrypted_char = chr(ord(char) - key)
        decrypted_text += decrypted_char
    
    return decrypted_text

input_text = "Hello, world!"
key = 5

encrypted_text = encrypt_text(input_text, key)
print("加密后的文本：", encrypted_text)

decrypted_text = decrypt_text(encrypted_text, key)
print("解密后的文本：", decrypted_text)
