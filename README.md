from time import sleep
import sys

def print_lirik():
    lines = [
        ("hallowwww", 0.07),  # Mengurangi delay karakter
        ("apa kabar kamuuu?", 0.07),
        ("mudahan kamu baik yaaaaaa", 0.07),
        ("oh ya semoga hari kamu selalu menyenangkan", 0.07),
        ("mudah mudahan kita bisa ketemu yaaa", 0.05),
        ("i miss you", 0.07),
        ("kalopun kamu ngga kangen aku ngga papa kok", 0.07),
        ("i stil miss you in univers wkwkwkwk", 0.07),
        ("maaf ya aku banyak salah sama kamu", 0.07),
        ("mudahan kamu maafin aku", 0.07),
        ("oh ya semoga hari hari mu bahgia", 0.07),
        ("salam hangat dari aku untuk kamu", 0.07)
    ]

    delays = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.3, 0.3, 0.5, 0.5, 0.5, 0.5]  # Mempercepat delay antar baris

    for i, (line, char_delay) in enumerate(lines):
        for char in line:
            print(char, end='', flush=True)
            sleep(char_delay)
        sleep(delays[i])
        print()

print_lirik()
