#
# Auto-generated sample makefile
#
# This makefile is intended for use with GNU make.
# Set the paths to the tools (CC, AR, LD, etc.)
#

CC = gcc
AR = ar

.PHONY: clean all

DEFINES = -D NUM_OUTPUT_CHANNELS=2 -D _SAMPLE_RATE_44100 -D MAX_SYNTH_VOICES=64 \
	  -D EAS_WT_SYNTH -D _8_BIT_SAMPLES -D _FILTER_ENABLED  \
	  -D _WAVE_PARSER -D MAX_SMF_STREAMS=32 \
	  -D _REVERB_ENABLED -D _CHORUS_ENABLED -D DLS_SYNTHESIZER \
	  -D MMAPI_SUPPORT -D UNIFIED_DEBUG_MESSAGES \
	  -D _IMELODY_PARSER -D _RTTTL_PARSER -D _OTA_PARSER -D _XMF_PARSER

OBJS = eas_mididata.o eas_pan.o eas_wavefiledata.o \
       eas_reverb.o eas_mdls.o eas_mixbuf.o eas_tcdata.o eas_chorus.o eas_pcmdata.o \
       eas_math.o eas_tonecontrol.o eas_voicemgt.o eas_public.o eas_dlssynth.o eas_midi.o \
       eas_flog.o eas_wtengine.o eas_imaadpcm.o eas_wtsynth.o eas_pcm.o eas_mixer.o \
       eas_wavefile.o eas_ima_tables.o eas_data.o eas_config.o eas_report.o eas_hostmm.o \
       eas_smf.o eas_smfdata.o eas_imelody.o eas_imelodydata.o eas_ota.o eas_otadata.o \
       eas_rtttl.o  eas_rtttldata.o eas_xmf.o eas_xmfdata.o

all: libsonicvox.a
       
libsonicvox.a: $(OBJS)
	$(AR) cr $@ $(OBJS)

clean:
	-rm $(OBJS) libsonicvox.a

%.o: %.c
	$(CC) -c -Wall -O2 -o $@ -I ../include $(DEFINES) $<
	