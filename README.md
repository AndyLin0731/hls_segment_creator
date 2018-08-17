# hls_segment_creator
a cross-platform m3u8 &amp; ts file creator


ffmpeg generate hls_segment(ts) command as follows:

ffmpeg -y -i 0.h264 -flags -global_header -f segment -segment_list ht1.m3u8 -segment_time 10 -segment_format mpeg_ts -segment_list_type m3u8 ht1__%05d.ts
ffmpeg -y -i 1.h264 -flags -global_header -f segment -segment_list ht1.m3u8 -segment_time 10 -segment_format mpeg_ts -segment_list_type m3u8 ht1__%05d.ts
