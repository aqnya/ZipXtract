cmake_minimum_required(VERSION 3.4.1)

add_library(p7zip SHARED
    CPP/7zip/Common/MyString.cpp
    CPP/7zip/Common/MyWindows.cpp
    CPP/7zip/Common/MyVector.cpp
    CPP/7zip/Common/StringConvert.cpp
    CPP/7zip/Common/Wildcard.cpp
    CPP/7zip/Common/ListFileUtils.cpp
    CPP/7zip/Common/StdInStream.cpp
    CPP/7zip/Common/StdOutStream.cpp
    CPP/7zip/Common/FileStreams.cpp
    CPP/7zip/Common/StreamUtils.cpp
    CPP/7zip/Common/CRC.cpp
    CPP/7zip/Compress/LzmaDecoder.cpp
    CPP/7zip/Compress/LzmaEncoder.cpp
    CPP/7zip/Compress/Lzma2Decoder.cpp
    CPP/7zip/Compress/Lzma2Encoder.cpp
    CPP/7zip/Compress/Bcj2Coder.cpp
    CPP/7zip/Compress/BcjCoder.cpp
    CPP/7zip/Compress/BranchCoder.cpp
    CPP/7zip/Compress/CopyCoder.cpp
    CPP/7zip/Compress/DeflateDecoder.cpp
    CPP/7zip/Compress/DeflateEncoder.cpp
    CPP/7zip/Compress/PpmdDecoder.cpp
    CPP/7zip/Compress/PpmdEncoder.cpp
    CPP/7zip/Archive/7z/7zIn.cpp
    CPP/7zip/Archive/7z/7zOut.cpp
    CPP/7zip/Archive/7z/7zHandler.cpp
    CPP/7zip/Archive/7z/7zProperties.cpp
    CPP/7zip/Archive/Common/InStreamWithCRC.cpp
    CPP/7zip/Archive/Common/OutStreamWithCRC.cpp
    CPP/7zip/Archive/Common/ItemNameUtils.cpp
    CPP/7zip/Archive/Common/MultiStream.cpp
    CPP/7zip/Archive/Common/HandlerOut.cpp
    CPP/7zip/Archive/Common/FindSignature.cpp
)

include_directories(
    CPP/
    CPP/7zip/
    CPP/7zip/Archive/
    CPP/7zip/Archive/7z/
    CPP/7zip/Compress/
    CPP/7zip/Common/
)
