#!/usr/bin/python
__author__ = "nadeem"


def stopwords(input_terms,delimiter=";"):
    """Form a complex number.

    Arguments:
    input_terms -- the string containing terms seperated by delimiter
    delimiter -- delimiter seperating terms, default is semi-colon";"
    """
    terms=input_terms +delimiter
    terms = terms.split(delimiter)

    unique_terms = set()
    for t in terms:
      unique_terms.add(t.lower().strip())

    f = open('validwords.txt')
    words = set()
    for line in iter(f):
        words.add(line.lower().strip())

    
    return list(words.intersection(unique_terms))

if __name__ == "__main__":
    t = "Attention Deficit Disorder with Hyperactivity;Child Behavior;Personal Autonomy;Choice Behavior;Morals;Adolescent Behavior;Humans;Female;Central Nervous System Stimulants;Male"
    print stopwords(t)
