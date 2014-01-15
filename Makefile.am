ACLOCAL_AMFLAGS = -I ../fintp_utils/m4

lib_LTLIBRARIES = libfintp_ws.la

AM_CPPFLAGS = $(CFLAGS_INCL) \
@CPPFLAGS@	\
@XERCES_CPPFLAGS@ @XALAN_CPPFLAGS@	\
$(OPT_FLAGS)

LIBFLAGS = @LIBS@ @LDFLAGS@	\
@XERCES_LDFLAGS@ @XALAN_LDFLAGS@ -lxerces-c -lxalan-c

AUTOMAKE_OPTIONS = foreign

libfintp_ws_la_SOURCES = $(SRCS)
libfintp_ws_la_LDFLAGS = $(LIBFLAGS)

CFLAGS_INCL = -DUNIX -DDEBUG_ENABLED

SRCS = src/WSVersionInfo.cpp	\
src/SOAP/SoapHeader.cpp	\
src/WSRM/Ack.cpp	\
src/WSRM/AcknowledgementRange.cpp	\
src/WSRM/Nack.cpp	\
src/WSRM/SequenceAcknowledgement.cpp	\
src/WSRM/SequenceDistinctAck.cpp	\
src/WSRM/SequenceFault.cpp	\
src/WSRM/SequenceResponse.cpp	\
src/WSRM/SequenceType.cpp	\
src/WSSerializable.cpp	\
src/WSU/Identifier.cpp

nobase_include_HEADERS = src/SOAP/SoapHeader.h	\
src/WSRM/Ack.h	\
src/WSRM/AcknowledgementRange.h	\
src/WSRM/Nack.h	\
src/WSRM/SequenceAcknowledgement.h	\
src/WSRM/SequenceDistinctAck.h	\
src/WSRM/SequenceFault.h	\
src/WSRM/SequenceResponse.h	\
src/WSRM/SequenceType.h	\
src/WSSerializable.h	\
src/WSU/Identifier.h	\
src/XmlStringUtil.h
