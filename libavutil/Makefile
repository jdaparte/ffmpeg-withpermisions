include $(SUBDIR)../config.mak

NAME = avutil

HEADERS = adler32.h                                                     \
          aes.h                                                         \
          aes_ctr.h                                                     \
          attributes.h                                                  \
          audio_fifo.h                                                  \
          audioconvert.h                                                \
          avassert.h                                                    \
          avstring.h                                                    \
          avutil.h                                                      \
          base64.h                                                      \
          blowfish.h                                                    \
          bprint.h                                                      \
          bswap.h                                                       \
          channel_layout.h                                              \
          common.h                                                      \
          cpu.h                                                         \
          crc.h                                                         \
          encryption_info.h                                             \
          error.h                                                       \
          eval.h                                                        \
          fifo.h                                                        \
          file.h                                                        \
          hmac.h                                                        \
          imgutils.h                                                    \
          intfloat.h                                                    \
          intfloat_readwrite.h                                          \
          intreadwrite.h                                                \
          lfg.h                                                         \
          log.h                                                         \
          mathematics.h                                                 \
          md5.h                                                         \
          mem.h                                                         \
          dict.h                                                        \
          display.h                                                     \
          old_pix_fmts.h                                                \
          opt.h                                                         \
          parseutils.h                                                  \
          pixdesc.h                                                     \
          pixfmt.h                                                      \
          random_seed.h                                                 \
          rational.h                                                    \
          samplefmt.h                                                   \
          sha.h                                                         \
          spherical.h                                                   \
          time.h                                                        \
          timecode.h                                                    \
          timestamp.h                                                   \
          version.h                                                     \
          xtea.h                                                        \

HEADERS-$(CONFIG_LZO)                   += lzo.h

ARCH_HEADERS = bswap.h                                                  \
               intmath.h                                                \
               intreadwrite.h                                           \
               timer.h                                                  \

BUILT_HEADERS = avconfig.h

OBJS = adler32.o                                                        \
       aes.o                                                            \
       aes_ctr.o                                                        \
       audio_fifo.o                                                     \
       avstring.o                                                       \
       base64.o                                                         \
       blowfish.o                                                       \
       bprint.o                                                         \
       channel_layout.o                                                 \
       cpu.o                                                            \
       crc.o                                                            \
       des.o                                                            \
       encryption_info.o                                                \
       error.o                                                          \
       eval.o                                                           \
       fifo.o                                                           \
       file.o                                                           \
       float_dsp.o                                                      \
       hmac.o                                                           \
       imgutils.o                                                       \
       intfloat_readwrite.o                                             \
       intmath.o                                                        \
       lfg.o                                                            \
       lls.o                                                            \
       log.o                                                            \
       log2_tab.o                                                       \
       mathematics.o                                                    \
       md5.o                                                            \
       mem.o                                                            \
       dict.o                                                           \
       display.o                                                        \
       opt.o                                                            \
       parseutils.o                                                     \
       pixdesc.o                                                        \
       random_seed.o                                                    \
       rational.o                                                       \
       rc4.o                                                            \
       samplefmt.o                                                      \
       sha.o                                                            \
       spherical.o                                                      \
       time.o                                                           \
       timecode.o                                                       \
       tree.o                                                           \
       utils.o                                                          \
       xga_font_data.o                                                  \
       xtea.o                                                           \

OBJS-$(CONFIG_LZO)                      += lzo.o

OBJS += $(COMPAT_OBJS:%=../compat/%)

SKIPHEADERS          = old_pix_fmts.h

TESTPROGS = adler32                                                     \
            aes                                                         \
            avstring                                                    \
            base64                                                      \
            blowfish                                                    \
            bprint                                                      \
            cpu                                                         \
            crc                                                         \
            des                                                         \
            error                                                       \
            eval                                                        \
            file                                                        \
            fifo                                                        \
            hmac                                                        \
            lfg                                                         \
            lls                                                         \
            md5                                                         \
            opt                                                         \
            pca                                                         \
            parseutils                                                  \
            random_seed                                                 \
            rational                                                    \
            sha                                                         \
            tree                                                        \
            xtea                                                        \

TESTPROGS-$(HAVE_LZO1X_999_COMPRESS) += lzo

TOOLS = ffeval ffescape

$(SUBDIR)lzo-test$(EXESUF): ELIBS = -llzo2
