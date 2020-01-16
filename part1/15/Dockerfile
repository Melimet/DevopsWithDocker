FROM ubuntu

RUN apt-get update && apt-get install -y git python3.6 sqlite3 libsqlite3-dev python3-pip

RUN git clone https://github.com/Melimet/DiscussionForum.git

EXPOSE 5000

WORKDIR /DiscussionForum

RUN python3.6 -m pip install -r requirements.txt

CMD python3.6 run.py  