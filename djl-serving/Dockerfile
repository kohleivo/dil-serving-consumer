# cd djl-serving
# docker build -t kohleivo/djl-serving:latest .
# docker push kohleivo/djl-serving:latest

FROM --platform=linux/amd64 deepjavalibrary/djl-serving:0.36.0

# Copy Model
COPY *.zip /opt/ml/
RUN unzip /opt/ml/traced_resnet18.zip -d /opt/ml/model/traced_resnet18
RUN rm /opt/ml/traced_resnet18.zip
