# convai_docker


Install
1) clone this project
2) put glove in data/glove.840B.300d.txt
3) download model.zip from slack and extract to model directory
4) Edit model/da_cnn/checkpoints/checkpoint. Remove pathes except model-134900.
5) install nvidia-docker

How to run

1) sudo nvidia-docker run -w /app -p 1990:1990 -v {/path/to/convai_docker}:/app calee/kaib python run-demo-simple.py  --> https server execution

2) CC mode example
python get_answer_cnsl.py --paragraph "dummy" --question "who are you ?"

3) QA mode example
python get_answer_cnsl.py --paragraph "sample paragraph ha ha ha" --question "what is the name of sample paragraph ?"
