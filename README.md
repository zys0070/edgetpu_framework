# edgetpu_framework
edgetpu codes reading and customizeing


detect.py[main()] -> apps.py[run_app()] -> gstreamer.py[run_gen()]
-> detect.py[render_gen(): yield utils.input_image_size(engine) ] 
-> gstreamer.py[run()]
  -> gstreamer.py[get_pipeline()]
    -> gstreamer.py[make_layout()]
    -> gstreamer.py[camera_pipeline()/file_pipline()] -> pipelines.py[camera_display_pipeline()...] -> gst.py[Filter()...] -> pipelines.py[inference_pipeline()]
  -> gstreamer.py[run_pipeline()]