import requests
import os
import sys
import json


def postFun(data):
    url = "input the post url"
    #data = {'id' : 123}

    headers = {'content-type': application/json}

    res = rq.post(url=url, data=data, headers=deaders)
    traget = res.json()
    return target


def judgeWhite(jsonData):
    dicData = json.loads(jsonData)
    if dicData['parm1'] != '' and dicData['parm2'] != '':
        return True
    return False


def saveLocal(data):
    with open("writefilename", "a") as f:
        f.write(data)


def main():
    with open("readfilename", "r") as f:
        lines = f.readlines()
        data = {'id' : 123i,
                'others' : '...'}
        for line in lines:
            data['id'] = line
            res = postFun(data)
            if judgeWhite(res):
                saveLocal("the data you selected")


if __name__ == "__main__":
    main()
