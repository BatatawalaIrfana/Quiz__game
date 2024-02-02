questions=("Which of the following comes under combinational circuit?",
           "Which of the following is not a programming language?",
           "Full Adder has how many outputs?",
           "HTML has how many heading tags?",
           "How many types of loops are there in C++")

options=(('A)Half Adder','B)SR FF','C)JK FF','D)EX-OR GATE'),
         ('A)Java','B)C++','C)Python','D)HTML'),
         ('A)2','B)3','C)1','D)4'),
         ('A)4','B)2','C)6','D)5'),
         ('A)4','B)2','C)6','D)3'))

answers=("A","D","B","C","D")
guesses=[]
score=0
qeustion_num=0

for q in questions:
    print("-----------------------------")
    print("                      ")
    print(q)
    for o in options[qeustion_num]:
        print(o)

    guess=input("Enter (A,B,C,D):").upper()
    guesses.append(guess)
    if guess==answers[qeustion_num]:
        score+=1
        print("Correct")
    else:
        print("Incorrect")
        print(f"{answers[qeustion_num]} is the correct answer")
    
    qeustion_num=qeustion_num+1
    
score=int(score/len(questions)*100)
print("Your score is:",score,"%")

















