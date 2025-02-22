FROM python:3.13-slim

RUN python3 -m pip install --upgrade pip
ENV VIRTUAL_ENV=/opt/venv
RUN python3 -m venv $VIRTUAL_ENV
ENV PATH="$VIRTUAL_ENV/bin:$PATH"
ADD ./requirements.txt /
RUN pip install -r /requirements.txt

# RUN addgroup --system --gid 1001 appgroup && adduser --system --uid 1001 --ingroup appgroup appuser

# USER appuser

WORKDIR /app
COPY . /app

CMD ["tail", "-f", "/dev/null"]