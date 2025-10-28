import sys
import time

def jalanin_lirik():
    # Lirik lagu dan delay antar karakter
    lirik = [
        ("I never knew you were the someone waitin' for me", 0.05),
        ("'Cause we were just kids when we fell in love, not knowin' what it was", 0.05),
        ("I will not give you up this time", 0.05),
        ("Oh, darling, just kiss me slow, your heart is all I own", 0.05),
        ("And in your eyes, you're holding mine", 0.05),
        ("Baby, I'm dancin' in the dark with you between my arms", 0.05),
        ("Barefoot on the grass while listenin' to our favourite song", 0.05),
        ("When you said you looked a mess, I whispered underneath my breath", 0.05),
        ("But you heard it, 'Darling, you look perfect tonight'", 0.05),
    ]

    # Delay antar baris
    delay = [0.5] * len(lirik)

    # Judul lagu
    print("\n== Perfect - Ed Sheeran ==\n")

    # Menjalankan lirik dengan efek mengetik
    for i, (baris_lagu, delay_karakter) in enumerate(lirik):
        for karakter in baris_lagu:
            print(karakter, end='')
            sys.stdout.flush()
            time.sleep(delay_karakter)
        time.sleep(delay[i])
        print('')

# Jalankan fungsi
jalanin_lirik()

