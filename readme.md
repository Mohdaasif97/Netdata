# Netdata System Monitoring

I set up Netdata to monitor my system resources using Docker.

## Commands Used

```bash
# Run Netdata container
docker run -d --name=netdata -p 19999:19999 -v /var/run/docker.sock:/var/run/docker.sock:ro netdata/netdata

# Access dashboard
http://localhost:19999
```

## Dashboard Screenshots

![Apps](Apps.png) ![CPU](cpu.png) ![Disk](disk.png) ![Home](home.png) ![Metrics](metrics.png) ![Nodes](nodes.png) ![System](system.png)

The dashboard shows real-time monitoring of:
- CPU usage
- Memory consumption  
- Disk I/O
- System processes
- Docker containers
- Network metrics

## What I Monitored

I was able to view comprehensive system metrics including CPU performance, memory usage, disk activity, and running applications through the web-based dashboard interface.
