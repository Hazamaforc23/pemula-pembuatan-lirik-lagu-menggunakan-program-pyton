Lagu Lestari

import sys
from time import sleep

def print_lyrics():
    """
    Mencetak lirik secara bertahap, dengan jeda antar karakter dan antar baris.
    Setiap baris memiliki jeda antar karakter yang berbeda, serta jeda antar baris yang berbeda.
    """
    lyrics = [
        ("Sang dewi katon nglamlami", 0.06),
        ("Ambabar wewangi semi", 0.08),
        ("Arum kembange melathi", 0.07),
        ("Dhasar wulane ndadari", 0.06),

        ("Wong bagus setya rumeksa nala", 0.08),
        ("Sasat abyoring kartika", 0.06),
        ("Kadya puspita ing nendra", 0.07),
        ("Hanjangkepi tresna", 0.09),

        ("Rasa tresna kang sejati", 0.07),
        ("Manggiha lestari", 0.08),
        ("Angidung tembang suci", 0.06),
        ("Nyengsemi sakjroning sepi", 0.09),

        ("Cahyamu amadhangi saratri", 0.08),
        ("Dadya kembange ati", 0.05),
         
        ("Angen-angenku lelana tawang", 0.08),
        ("Mideri tanpa wangenan", 0.07),
        ("Lumaku nembus marang kabagyan", 0.09),
        ("Banget manis sinawang", 0.06),

        ("Wong bagus setya rumeksa nala", 0.06),
        ("Sasat abyoring kartika", 0.07),
        ("Kadya puspita ing nendra", 0.08),
        ("Hanjangkepi tresna", 0.09),

        ("Rasa tresna kang sejati", 0.08),
        ("Manggiha lestari", 0.07),
        ("Angidung tembang suci", 0.08),
        ("Nyengsemi sakjroning sepi", 0.09),

        ("Cahyamu amadhangi saratri", 0.07),
        ("Dadya kembange ati", 0.08),
        ("Rasa tresna kang sejati", 0.06),
        ("Manggiha lestari", 0.08),
        ("Angidung tembang suci", 0.09),
        ("Nyengsemi sakjroning sepi", 0.07),

        ("Cahyamu amadhangi saratri", 0.08),
        ("Dadya kembange ati", 0.09),

        ("Angen-angenku lelana tawang", 0.06),
        ("Mideri tanpa wangenan", 0.08),
        ("Lumaku nembus marang kabagyan", 0.09),
        ("Banget manis sinawang", 0.06),
        ("Wong manis sing tak sayang", 0.08),
    ]
    pauses = [1.1, 0.4, 2.7, 0.2] * ((len(lyrics) // 4) + 1)
    
    for i, (line, char_pause) in enumerate(lyrics):
        for char in line:
            print(char, end="")
            sys.stdout.flush()
            sleep(char_pause)
        print()  
        sleep(pauses[i])


print_lyrics()
