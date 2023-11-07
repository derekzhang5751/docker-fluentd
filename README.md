# docker-fluentd
Fluentd for log collection

# Build an image with Fluentd and fluent-plugin-mongo
$ docker build -t fluent-mongo-image .

# Create account in MongoDB
$ use fluentd

$ db.createUser({
    user: "fluentd",
    pwd: "fluentd",
    roles: [{ role: "readWrite", db: "fluentd" }]
})
