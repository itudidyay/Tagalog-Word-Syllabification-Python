# Tagalog-Word-Syllabification-Python

This program breaks down Tagalog words into syllables.

Usage
--------------------
    >>> syllabize('Tagalog')
    ['Ta', 'ga', 'log']
    >>> wordList = ['ube', 'tao', 'noón', 'bahay', 'nauuhaw', 'aklát', 'titser', 'eksperto', 'inspirasyón', 'silindro', 'templo', 'instruksyón', 'éksplosibo', 'ékstraordináryo']
    >>> for word in wordList:
    >>>   print(word, syllabify(word))
    ube ['u', 'be']
    tao ['ta', 'o']
    noón ['no', 'ón']
    bahay ['ba', 'hay']
    nauuhaw ['na', 'u', 'u', 'haw']
    aklát ['ak', 'lát']
    titser ['tit', 'ser']
    eksperto ['eks', 'per', 'to']
    inspirasyón ['ins', 'pi', 'ras', 'yón']
    silindro ['si', 'lin', 'dro']
    templo ['tem', 'plo']
    instruksyón ['ins', 'truks', 'yón']
    éksplosibo ['éks', 'plo', 'si', 'bo']
    ékstraordináryo ['éks', 'tra', 'or', 'di', 'nár', 'yo']
    
How does it work?
--------------------
According to KFW Manwal sa Masinop na Pagsulat [https://kwf.gov.ph/wp-content/uploads/MMP_Full.pdf], the rules of syllabification in Tagalog are as follows,

1. If there are two or more consecutive vowels, they are separated. Example: /a•ak•yat/ (aakyat), /to•to•o/ (totoo)
2. If there are two consecutive constants, they are separated. Example: /tit•ser/ (titser), /ak•lat/ (aklat)
3. If there are three consecutive constants, and the first of the constants is an N or M, and the second and third are BL, BR, DR, PL, at TR, then the first constant joins the previous syllable, and the second and third join the following syllable. Example: /sen•tro/ (sentro), /tim•bre/ (timbre)
4. If there are three consecutive constants, and they don't follow the above conditions, then the first and second constant join the previous syllable, and the third joins the following syllable. Example: /trans•fer/ (transfer), /ins•pi•ras•yon/ (inspirasyon)
5. If there are four or more consecutive vowels, the first and second join the previous syllable, and the rest join the following syllable. Example: /des•kons•truk•si•yón/ (deskonstruksiyón), /trans•plant/ (transplant)
