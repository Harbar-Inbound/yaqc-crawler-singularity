Bootstrap: docker
From: yaqc/crawler:v0.4.0

%post
    echo 'export PROJECT_NAME="yaqc"' >>$SINGULARITY_ENVIRONMENT
    echo 'export RABBITMQ_USER="yaqc"' >>$SINGULARITY_ENVIRONMENT
    echo 'export PROJECT_ENVIRONMENT="develop"' >>$SINGULARITY_ENVIRONMENT

%apprun crawler
exec python /app/crawler.py