### Installing

A step by step series of examples that tell you how to get a development env running

1. Install all the requirements

```
pip install -r requirements.txt
```

2. Start the viewer, on the server.

```
python StreamViewer.py
```

3. On another machine connected to the same network, start the streamer, and enter the IP of the machine running the StreamViewer.

```
python Streamer.py -s 192.168.1.X
```

You will see the video being streamed across the network to your Viewer.

## Running the tests (WebCam Needed)

```
python -m unittest discover .
```

1. `test_camera.py` - Tests if camera can be detected with OpenCV

   `python -m unittest camera.test_camera`

2. `test_local_streaming.py` - Tests Streaming and Viewing silently locally

   `python -m unittest test_local_streaming`
