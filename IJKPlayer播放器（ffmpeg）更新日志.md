#IJKPlayer播放器更新日志

tag k0.7.6
```
ffmpeg: ass subtitle support
msg_queue: add resource for msg_queue
ios: separate vtb sync mode from mixed vtb
android: fix some thread competition
android: support setSpeed for pre-M(api<23) versions
```
tag k0.7.5
```
ffmpeg: disable-asm on architecture x86
ffmpeg: revert some cutted demuxer and decoder
ios: add playback volume interface
```
tag k0.7.4
```
ffplay: fix sample buffer leak introduced in k0.7.1
doc: add takeoff checklist
```
tag k0.7.3
```
ios: turn videotoolbox into singleton
ffmpeg: merge ipv6 issue in tcp.c
```
tag k0.7.2
```
ios: fix a compile error
```
tag k0.7.1
```
ffmpeg: upgrade to n3.2
```
tag k0.6.3
```
ffmpeg: disable clock_gettime added in xcode8
android: make NDKr13 happy
Raw Blame History
Watch 778 Unstar 10,437 Fork 3,345
```
tag k0.6.2
```
ffmpeg: fix wild pointer when decoder was not found
player: fix bug introduced in k0.6.0
```
tag k0.6.1
```
concat: fix crash introduced in k0.6.0
flvdec: fix seek problem introduced in k0.6.0
hls: fix regression with ranged media segments
```
tag k0.6.0
```
openssl: upgrade to 1.0.2h
ffmpeg: upgrade to n3.1
MediaCodec: add options to enable resolution change.
VideoToolbox: add options to enable resolution change.
```
tag k0.5.1
```
ffmpeg: fix crash introduced in k0.5.0
```
tag k0.5.0
```
ffmpeg: upgrade to n3.0
android: support NDKr11
```
tag k0.4.5
```
ios: support playbackRate change. (iOS 7.0 or later)
android: support speed change. (Android 6.0 or later)
player: do not link avfilter by default.
android: add x86_64 support
android: move jjk out to jni4android project
android: support OpenGL ES2 render
```
tag k0.4.4
```
ios: replace MPMoviePlayerXXX with IJKMPMoviePlayerXXX
ios: remove target 'IjkMediaPlayer'. 'IjkMediaFramework' should be used instead.
android: switch ExoPlayer to r1.5.2
```
tag k0.4.3
```
android: fix several crash when reconfiguring MediaCodec
android: add jjk to generate API native wrapper
android: support IMediaDataSource for user to supply media data
```
tag k0.4.2
```
ios: support Xcode 7
ios: drop support of iOS 5.x
ffmpeg: enable libavfilter
player: limited support of libavfilter
android: add ExoPlayer as an alternative backend player
```
tag k0.4.1
```
android: support downloading from jcenter
```
tag k0.4.0
```
ffmpeg: switch to ffmpeg n2.8
```


#FFMPEG更新日志

version <3.2.1>:
```
- CrystalHD decoder moved to new decode API
- add internal ebur128 library, remove external libebur128 dependency
- Pro-MPEG CoP #3-R2 FEC protocol
- premultiply video filter
- Support for spherical videos
- configure now fails if autodetect-libraries are requested but not found
- PSD Decoder
- 16.8 floating point pcm decoder
- 24.0 floating point pcm decoder
- Apple Pixlet decoder
- QDMC audio decoder
```
version 3.2:
```
- libopenmpt demuxer
- tee protocol
- Changed metadata print option to accept general urls
- Alias muxer for Ogg Video (.ogv)
- VP8 in Ogg muxing
- curves filter doesn't automatically insert points at x=0 and x=1 anymore
- 16-bit support in curves filter and selectivecolor filter
- OpenH264 decoder wrapper
- MediaCodec H.264/HEVC/MPEG-4/VP8/VP9 hwaccel
- True Audio (TTA) muxer
- crystalizer audio filter
- acrusher audio filter
- bitplanenoise video filter
- floating point support in als decoder
- fifo muxer
- maskedclamp filter
- hysteresis filter
- lut2 filter
- yuvtestsrc filter
- CUDA CUVID H.263/VP8/VP9/10 bit HEVC (Dithered) Decoding
- vaguedenoiser filter
- added threads option per filter instance
- weave filter
- gblur filter
- avgblur filter
- sobel and prewitt filter
- MediaCodec HEVC/MPEG-4/VP8/VP9 decoding
- Meridian Lossless Packing (MLP) / TrueHD encoder
- Non-Local Means (nlmeans) denoising filter
- sdl2 output device and ffplay support
- sdl1 output device and sdl1 support removed
- extended mov edit list support
- libfaac encoder removed
- Matroska muxer now writes CRC32 elements by default in all Level 1 elements
- sidedata video and asidedata audio filter
- Changed mapping of rtp MIME type G726 to codec g726le.
- spec compliant VAAPI/DXVA2 VC-1 decoding of slices in frame-coded images
```
version 3.1:
```
- DXVA2-accelerated HEVC Main10 decoding
- fieldhint filter
- loop video filter and aloop audio filter
- Bob Weaver deinterlacing filter
- firequalizer filter
- datascope filter
- bench and abench filters
- ciescope filter
- protocol blacklisting API
- MediaCodec H264 decoding
- VC-2 HQ RTP payload format (draft v1) depacketizer and packetizer
- VP9 RTP payload format (draft v2) packetizer
- AudioToolbox audio decoders
- AudioToolbox audio encoders
- coreimage filter (GPU based image filtering on OSX)
- libdcadec removed
- bitstream filter for extracting DTS core
- ADPCM IMA DAT4 decoder
- musx demuxer
- aix demuxer
- remap filter
- hash and framehash muxers
- colorspace filter
- hdcd filter
- readvitc filter
- VAAPI-accelerated format conversion and scaling
- libnpp/CUDA-accelerated format conversion and scaling
- Duck TrueMotion 2.0 Real Time decoder
- Wideband Single-bit Data (WSD) demuxer
- VAAPI-accelerated H.264/HEVC/MJPEG encoding
- DTS Express (LBR) decoder
- Generic OpenMAX IL encoder with support for Raspberry Pi
- IFF ANIM demuxer & decoder
- Direct Stream Transfer (DST) decoder
- loudnorm filter
- MTAF demuxer and decoder
- MagicYUV decoder
- OpenExr improvements (tile data and B44/B44A support)
- BitJazz SheerVideo decoder
- CUDA CUVID H264/HEVC decoder
- 10-bit depth support in native utvideo decoder
- libutvideo wrapper removed
- YUY2 Lossless Codec decoder
- VideoToolbox H.264 encoder
```
version 3.0:
```
- Common Encryption (CENC) MP4 encoding and decoding support
- DXV decoding
- extrastereo filter
- ocr filter
- alimiter filter
- stereowiden filter
- stereotools filter
- rubberband filter
- tremolo filter
- agate filter
- chromakey filter
- maskedmerge filter
- Screenpresso SPV1 decoding
- chromaprint fingerprinting muxer
- ffplay dynamic volume control
- displace filter
- selectivecolor filter
- extensive native AAC encoder improvements and removal of experimental flag
- ADPCM PSX decoder
- 3dostr, dcstr, fsb, genh, vag, xvag, ads, msf, svag & vpk demuxer
- zscale filter
- wve demuxer
- zero-copy Intel QSV transcoding in ffmpeg
- shuffleframes filter
- SDX2 DPCM decoder
- vibrato filter
- innoHeim/Rsupport Screen Capture Codec decoder
- ADPCM AICA decoder
- Interplay ACM demuxer and audio decoder
- XMA1 & XMA2 decoder
- realtime filter
- anoisesrc audio filter source
- IVR demuxer
- compensationdelay filter
- acompressor filter
- support encoding 16-bit RLE SGI images
- apulsator filter
- sidechaingate audio filter
- mipsdspr1 option has been renamed to mipsdsp
- aemphasis filter
- mips32r5 option has been removed
- mips64r6 option has been removed
- DXVA2-accelerated VP9 decoding
- SOFAlizer: virtual binaural acoustics filter
- VAAPI VP9 hwaccel
- audio high-order multiband parametric equalizer
- automatic bitstream filtering
- showspectrumpic filter
- libstagefright support removed
- spectrumsynth filter
- ahistogram filter
- only seek with the right mouse button in ffplay
- toggle full screen when double-clicking with the left mouse button in ffplay
- afftfilt filter
- convolution filter
- libquvi support removed
- support for dvaudio in wav and avi
- libaacplus and libvo-aacenc support removed
- Cineform HD decoder
- new DCA decoder with full support for DTS-HD extensions
- significant performance improvements in Windows Television (WTV) demuxer
- nnedi deinterlacer
- streamselect video and astreamselect audio filter
- swaprect filter
- metadata video and ametadata audio filter
- SMPTE VC-2 HQ profile support for the Dirac decoder
- SMPTE VC-2 native encoder supporting the HQ profile
```
version 2.8:
```
- colorkey video filter
- BFSTM/BCSTM demuxer
- little-endian ADPCM_THP decoder
- Hap decoder and encoder
- DirectDraw Surface image/texture decoder
- ssim filter
- optional new ASF demuxer
- showvolume filter
- Many improvements to the JPEG 2000 decoder
- Go2Meeting decoding support
- adrawgraph audio and drawgraph video filter
- removegrain video filter
- Intel QSV-accelerated MPEG-2 video and HEVC encoding
- Intel QSV-accelerated MPEG-2 video and HEVC decoding
- Intel QSV-accelerated VC-1 video decoding
- libkvazaar HEVC encoder
- erosion, dilation, deflate and inflate video filters
- Dynamic Audio Normalizer as dynaudnorm filter
- Reverse video and areverse audio filter
- Random filter
- deband filter
- AAC fixed-point decoding
- sidechaincompress audio filter
- bitstream filter for converting HEVC from MP4 to Annex B
- acrossfade audio filter
- allyuv and allrgb video sources
- atadenoise video filter
- OS X VideoToolbox support
- aphasemeter filter
- showfreqs filter
- vectorscope filter
- waveform filter
- hstack and vstack filter
- Support DNx100 (1440x1080@8)
- VAAPI hevc hwaccel
- VDPAU hevc hwaccel
- framerate filter
- Switched default encoders for webm to VP9 and Opus
- Removed experimental flag from the JPEG 2000 encoder
```
version 2.7:
```
- FFT video filter
- TDSC decoder
- DTS lossless extension (XLL) decoding (not lossless, disabled by default)
- showwavespic filter
- DTS decoding through libdcadec
- Drop support for nvenc API before 5.0
- nvenc HEVC encoder
- Detelecine filter
- Intel QSV-accelerated H.264 encoding
- MMAL-accelerated H.264 decoding
- basic APNG encoder and muxer with default extension "apng"
- unpack DivX-style packed B-frames in MPEG-4 bitstream filter
- WebM Live Chunk Muxer
- nvenc level and tier options
- chorus filter
- Canopus HQ/HQA decoder
- Automatically rotate videos based on metadata in ffmpeg
- improved Quickdraw compatibility
- VP9 high bit-depth and extended colorspaces decoding support
- WebPAnimEncoder API when available for encoding and muxing WebP
- Direct3D11-accelerated decoding
- Support Secure Transport
- Multipart JPEG demuxer
```
version 2.6:
```
- nvenc encoder
- 10bit spp filter
- colorlevels filter
- RIFX format for *.wav files
- RTP/mpegts muxer
- non continuous cache protocol support
- tblend filter
- cropdetect support for non 8bpp, absolute (if limit >= 1) and relative (if limit < 1.0) threshold
- Camellia symmetric block cipher
- OpenH264 encoder wrapper
- VOC seeking support
- Closed caption Decoder
- fspp, uspp, pp7 MPlayer postprocessing filters ported to native filters
- showpalette filter
- Twofish symmetric block cipher
- Support DNx100 (960x720@8)
- eq2 filter ported from libmpcodecs as eq filter
- removed libmpcodecs
- Changed default DNxHD colour range in QuickTime .mov derivatives to mpeg range
- ported softpulldown filter from libmpcodecs as repeatfields filter
- dcshift filter
- RTP depacketizer for loss tolerant payload format for MP3 audio (RFC 5219)
- RTP depacketizer for AC3 payload format (RFC 4184)
- palettegen and paletteuse filters
- VP9 RTP payload format (draft 0) experimental depacketizer
- RTP depacketizer for DV (RFC 6469)
- DXVA2-accelerated HEVC decoding
- AAC ELD 480 decoding
- Intel QSV-accelerated H.264 decoding
- DSS SP decoder and DSS demuxer
- Fix stsd atom corruption in DNxHD QuickTimes
- Canopus HQX decoder
- RTP depacketization of T.140 text (RFC 4103)
- Port MIPS optimizations to 64-bit
```
version 2.5:
```
- HEVC/H.265 RTP payload format (draft v6) packetizer
- SUP/PGS subtitle demuxer
- ffprobe -show_pixel_formats option
- CAST128 symmetric block cipher, ECB mode
- STL subtitle demuxer and decoder
- libutvideo YUV 4:2:2 10bit support
- XCB-based screen-grabber
- UDP-Lite support (RFC 3828)
- xBR scaling filter
- AVFoundation screen capturing support
- ffserver supports codec private options
- creating DASH compatible fragmented MP4, MPEG-DASH segmenting muxer
- WebP muxer with animated WebP support
- zygoaudio decoding support
- APNG demuxer
- postproc visualization support
```
version 2.4:
```
- Icecast protocol
- ported lenscorrection filter from frei0r filter
- large optimizations in dctdnoiz to make it usable
- ICY metadata are now requested by default with the HTTP protocol
- support for using metadata in stream specifiers in fftools
- LZMA compression support in TIFF decoder
- H.261 RTP payload format (RFC 4587) depacketizer and experimental packetizer
- HEVC/H.265 RTP payload format (draft v6) depacketizer
- added codecview filter to visualize information exported by some codecs
- Matroska 3D support thorugh side data
- HTML generation using texi2html is deprecated in favor of makeinfo/texi2any
- silenceremove filter
```



