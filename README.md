# FileManipulation
Group files on json style -- a coding interview task

A good practice on tuple, dictionary, array

## Discription

'''

You are giving three input file path and one output file path, your task is to processing three input files and merge them into one. The three files separately contain a list of questions, answers or a list of group labels, and they are marked with a unique group id. The info in each line is split by a symbol "##".

Question file format:

group id(Integer),question id(Integer),question(String)(this line is not in the file)

123##1##how is the weather today.

123##2##what's the weather like today.

234##3##what's your name?

answer file format:

group id(Integer),answer id(Integer), answer(String)(this line is not in the file)

123##1##it is hot.

123##2##it is raining.

234##3##my name is doudou.


group file format:

group id(Integer),group label(String)(this line is not in the file)

123##weather

234##corpus

Requirements:

1. You are required to create a list of group, each group element including id, answer, question,and label. You will need to define a json schema, and output them into a file.

2. If you have no idea of json, that's fine. But be sure to merge the data into a data structure, like dict, list... whatever.

3. Please remove all spaces at front or end of question/answer.

4. some question or answer may not have group info in group file, handle this case by yourself.

'''

question_path = "./question.txt"

answer_path = "./answer.txt"

group_path = "./group.txt"

output_path = "./merged.txt"

