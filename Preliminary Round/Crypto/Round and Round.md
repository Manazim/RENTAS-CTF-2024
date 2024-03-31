# Description

For this question we need to decipher the ciphertext given.

![Screenshot 2024-03-31 120154](https://github.com/Manazim/RENTAS-CTF-2024/assets/97380455/14f8c9f0-e389-41a1-acbf-bc71bbc7cea7)

# Idea

The clues are round as mentioned on the title of the challenge, other than that, the description of the task also mentioned about pizza.
So just use Mr.Google to search the related cipher. First I tried to search for a round cipher but found nothing, then I tried to search for a Spiral cipher and found this cipher.

![image](https://github.com/Manazim/RENTAS-CTF-2024/assets/97380455/047567e9-3b36-4d44-9ecb-3257970acf34)

# Solution

We just need to understand the pattern of the ciphertext. We should subtract the number of the ciphertext with the constant value. The result of the subtraction cannot be less than the constant value. The selection of the number can be made up of 1 digit or 2 digits.

For example:

Our constant is 3.

21-3 = 18  #(18 is not less than 3)

18 = R  #(According to the spiral cipher image above)

Continue until you find the full flag with the same constant value.

RWSC{PIZZINI_CIPHER_WAS_EAZY}
