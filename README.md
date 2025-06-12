
import random
import string

def generate_password(length=12):
    """Generate a random password with letters, digits, and punctuation."""
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Example usage
print("Generated password:", generate_password(12))
