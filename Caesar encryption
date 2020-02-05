#Реализуйте функцию caesar(text, key), возвращающую зашифрованный текст, работающую только с латинским алфавитом.

#text - исходных текст, который надо зашифровать (или расшифровать)
#key - ключ (сдвиг)
#Ключ может быть отрицательным или больше 26

#Из преобразуемого текста удаляются все пробелы и знаки препинания. Зашифрованный текст пишется в верхнем регистре 1 строкой.

 

 

#Примечание. В этой задаче не нужно ничего считывать и ничего выводить на печать. Только реализовать функцию.
def caesar(text, key):
    text = text.replace(",","")
    text = text.replace(" ", "")
    text = text.replace("\'", "")
    text = text.replace(".", "")
    text = text.replace("'", "")
    text = text.upper()
    alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
    result_crypt = ""
    for t in text:
        i = alphabet.index(t)
        new_i = i + key
        while new_i < 0 or new_i > len(alphabet)-1:
            if new_i < 0:
                new_i = len(alphabet)+new_i
            if new_i > len(alphabet)-1:
                new_i = new_i-(len(alphabet))
        result_crypt += alphabet[new_i]
    return(result_crypt)
