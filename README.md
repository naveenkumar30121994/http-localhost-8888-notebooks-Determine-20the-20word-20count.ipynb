# http-localhost-8888-notebooks-Determine-20the-20word-20count.ipynb
Text="""
bands which have connected them with another, and to assume among the powers of the earth, the separate and equal station to which the Laws of Nature and of Nature's God entitle them, a decent respect to the opinions of mankind requires that they should declare the causes which impel them to the separation.  We hold these truths to be
self-evident, that all men are created equal, that they are endowed by their Creator with certain unalienable Rights, that among these are Life, Liberty and the pursuit of Happiness.--That to secure these rights, Governments are instituted among Men, deriving their just powers from the consent of the governed, --That whenever any Form of Government becomes destructive of these ends, it is the Right of the People to alter or to abolish it, and to institute new Government, laying its foundation on such principles and organizing its powers in such form, as to them shall seem most likely to effect their Safety and Happiness. """

# Cleaning text and lower casing all words
for char in '-.,\n':
    Text=Text.replace(char,' ')
Text = Text.lower()
# arrange returns a list of words delimited by sequences of whitespace (including tabs, newlines, etc, like re's \s) 
word_list = Text.arrange()

print (Text)

bands which have connected them with another, and to assume among the powers of the earth, the separate and equal station to which the Laws of Nature and of Nature's God entitle them, a decent respect to the opinions of mankind requires that they should declare the causes which impel them to the separation.  We hold these truths to be
self-evident, that all men are created equal, that they are endowed by their Creator with certain unalienable Rights, that among these are Life, Liberty and the pursuit of Happiness.--That to secure these rights, Governments are instituted among Men, deriving their just powers from the consent of the governed, --That whenever any Form of Government becomes destructive of these ends, it is the Right of the People to alter or to abolish it, and to institute new Government, laying its foundation on such principles and organizing its powers in such form, as to them shall seem most likely to effect their Safety and Happiness. 

bands which have connected them with another, and to assume among the powers of the earth, the separate and equal station to which the Laws of Nature and of Nature's God entitle them, a decent respect to the opinions of mankind requires that they should declare the causes which impel them to the separation.  We hold these truths to be
self-evident, that all men are created equal, that they are endowed by their Creator with certain unalienable Rights, that among these are Life, Liberty and the pursuit of Happiness.--That to secure these rights, Governments are instituted among Men, deriving their just powers from the consent of the governed, --That whenever any Form of Government becomes destructive of these ends, it is the Right of the People to alter or to abolish it, and to institute new Government, laying its foundation on such principles and organizing its powers in such form, as to them shall seem most likely to effect their Safety and Happiness. 
# split returns a list of words delimited by sequences of whitespace (including tabs, newlines, etc, like re's \s) 
word_list = Text.split()
print (word_list)
['bands', 'which', 'have', 'connected', 'them', 'with', 'another,', 'and', 'to', 'assume', 'among', 'the', 'powers', 'of', 'the', 'earth,', 'the', 'separate', 'and', 'equal', 'station', 'to', 'which', 'the', 'Laws', 'of', 'Nature', 'and', 'of', "Nature's", 'God', 'entitle', 'them,', 'a', 'decent', 'respect', 'to', 'the', 'opinions', 'of', 'mankind', 'requires', 'that', 'they', 'should', 'declare', 'the', 'causes', 'which', 'impel', 'them', 'to', 'the', 'separation.', 'We', 'hold', 'these', 'truths', 'to', 'be', 'self-evident,', 'that', 'all', 'men', 'are', 'created', 'equal,', 'that', 'they', 'are', 'endowed', 'by', 'their', 'Creator', 'with', 'certain', 'unalienable', 'Rights,', 'that', 'among', 'these', 'are', 'Life,', 'Liberty', 'and', 'the', 'pursuit', 'of', 'Happiness.--That', 'to', 'secure', 'these', 'rights,', 'Governments', 'are', 'instituted', 'among', 'Men,', 'deriving', 'their', 'just', 'powers', 'from', 'the', 'consent', 'of', 'the', 'governed,', '--That', 'whenever', 'any', 'Form', 'of', 'Government', 'becomes', 'destructive', 'of', 'these', 'ends,', 'it', 'is', 'the', 'Right', 'of', 'the', 'People', 'to', 'alter', 'or', 'to', 'abolish', 'it,', 'and', 'to', 'institute', 'new', 'Government,', 'laying', 'its', 'foundation', 'on', 'such', 'principles', 'and', 'organizing', 'its', 'powers', 'in', 'such', 'form,', 'as', 'to', 'them', 'shall', 'seem', 'most', 'likely', 'to', 'effect', 'their', 'Safety', 'and', 'Happiness.']
# 1. using for loops

# Initializing Dictionary
d = {}

# counting number of times each word comes up in list of words (in dictionary)
for word in word_list: 
    d[word] = d.get(word, 0) + 1
d
[(1, 'bands'),
 (3, 'which'),
 (1, 'have'),
 (1, 'connected'),
 (3, 'them'),
 (2, 'with'),
 (1, 'another,'),
 (7, 'and'),
 (11, 'to'),
 (1, 'assume'),
 (3, 'among'),
 (12, 'the'),
 (3, 'powers'),
 (9, 'of'),
 (1, 'earth,'),
 (1, 'separate'),
 (1, 'equal'),
 (1, 'station'),
 (1, 'Laws'),
 (1, 'Nature'),
 (1, "Nature's"),
 (1, 'God'),
 (1, 'entitle'),
 (1, 'them,'),
 (1, 'a'),
 (1, 'decent'),
 (1, 'respect'),
 (1, 'opinions'),
 (1, 'mankind'),
 (1, 'requires'),
 (4, 'that'),
 (2, 'they'),
 (1, 'should'),
 (1, 'declare'),
 (1, 'causes'),
 (1, 'impel'),
 (1, 'separation.'),
 (1, 'We'),
 (1, 'hold'),
 (4, 'these'),
 (1, 'truths'),
 (1, 'be'),
 (1, 'self-evident,'),
 (1, 'all'),
 (1, 'men'),
 (4, 'are'),
 (1, 'created'),
 (1, 'equal,'),
 (1, 'endowed'),
 (1, 'by'),
 (3, 'their'),
 (1, 'Creator'),
 (1, 'certain'),
 (1, 'unalienable'),
 (1, 'Rights,'),
 (1, 'Life,'),
 (1, 'Liberty'),
 (1, 'pursuit'),
 (1, 'Happiness.--That'),
 (1, 'secure'),
 (1, 'rights,'),
 (1, 'Governments'),
 (1, 'instituted'),
 (1, 'Men,'),
 (1, 'deriving'),
 (1, 'just'),
 (1, 'from'),
 (1, 'consent'),
 (1, 'governed,'),
 (1, '--That'),
 (1, 'whenever'),
 (1, 'any'),
 (1, 'Form'),
 (1, 'Government'),
 (1, 'becomes'),
 (1, 'destructive'),
 (1, 'ends,'),
 (1, 'it'),
 (1, 'is'),
 (1, 'Right'),
 (1, 'People'),
 (1, 'alter'),
 (1, 'or'),
 (1, 'abolish'),
 (1, 'it,'),
 (1, 'institute'),
 (1, 'new'),
 (1, 'Government,'),
 (1, 'laying'),
 (2, 'its'),
 (1, 'foundation'),
 (1, 'on'),
 (2, 'such'),
 (1, 'principles'),
 (1, 'organizing'),
 (1, 'in'),
 (1, 'form,'),
 (1, 'as'),
 (1, 'shall'),
 (1, 'seem'),
 (1, 'most'),
 (1, 'likely'),
 (1, 'effect'),
 (1, 'Safety'),
 (1, 'Happiness.')]
