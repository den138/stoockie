FROM public.ecr.aws/lambda/python:3.9

COPY requirements.txt ${LAMBDA_TASK_ROOT}

RUN pip install -r requirements.txt

COPY stoockie.py config.py ${LAMBDA_TASK_ROOT}

CMD [ "stoockie.handler" ]