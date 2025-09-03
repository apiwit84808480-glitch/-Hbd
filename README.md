import time
import random
import os

name = "โอห์ม"
age = int(input()) 

COLORS = ["\033[91m", "\033[92m", "\033[93m","\033[94m", "\033[95m", "\033[96m",]
RESET = "\033[0m" 

def slowly(text, delay=0.05):
    for ch in text:
        print(ch, end="", flush=True)
        time.sleep(delay)
    print()

def Good(lines=5, width=50):
    chars = "✦✧★☆❖❇❉✺✹♢♦•◦✨🎉"
    for _ in range(lines):
        row = "".join(random.choice(COLORS) + random.choice(chars) + RESET for _ in range(width))
        print(row)
        time.sleep(0.1)

def cakeee(age):
    print(" " * 15 + "🕯️ " * 5)
    print(" " * 17 + f"   {age}   ")
    print(" " * 13 + "┌───────────────┐")
    print(" " * 13 + "|   H A P P Y   |")
    print(" " * 13 + "|   B I R T H   |")
    print(" " * 13 + "|   D A Y 🎂   |")
    print(" " * 13 + "└───────────────┘")
    print(" " * 13 + "       |   |     ")
    print(" " * 13 + "   ~~~~~~~~~~~~~   ")
    print(" " * 13 + f"   |  TO {name}  |")
    print(" " * 13 + "   ~~~~~~~~~~~~~   ")
    
def main():
    os.system("cls" if os.name == "nt" else "clear")

    print("=" * 60)
    slowly("🎉✨   H  A  P  P  Y     B  I  R  T  H  D  A  Y   ✨🎉", 0.03)
    print("=" * 60)

    print()
    slowly(f"สุขสันต์วันเกิดนะ {name} !! 🎂", 0.05)
    print()

    Good(8, 40)
    
    cakeee(age)

    print("=" * 60)
    print("   จากเพื่อนสุดโหดมึงเอง😎 ")
    print("=" * 60)

if __name__ == "__main__":
    main()

#อีFAt โอห์ม
