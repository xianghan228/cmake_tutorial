cmake_minimum_required(VERSION 3.12)
project(GetFilenameComponent)

message(STATUS ===========================================)

cmake_host_system_information(RESULT NUMBER_OF_LOGICAL_CORES QUERY NUMBER_OF_LOGICAL_CORES)
message(STATUS "NUMBER_OF_LOGICAL_CORES ==> ${NUMBER_OF_LOGICAL_CORES}")

cmake_host_system_information(RESULT NUMBER_OF_PHYSICAL_CORES QUERY NUMBER_OF_PHYSICAL_CORES)
message(STATUS "NUMBER_OF_PHYSICAL_CORES ==> ${NUMBER_OF_PHYSICAL_CORES}")

cmake_host_system_information(RESULT HOSTNAME QUERY HOSTNAME)
message(STATUS "HOSTNAME ==> ${HOSTNAME}")

cmake_host_system_information(RESULT FQDN QUERY FQDN)
message(STATUS "FQDN ==> ${FQDN}")

cmake_host_system_information(RESULT TOTAL_VIRTUAL_MEMORY QUERY TOTAL_VIRTUAL_MEMORY)
message(STATUS "TOTAL_VIRTUAL_MEMORY ==> ${TOTAL_VIRTUAL_MEMORY}")

cmake_host_system_information(RESULT AVAILABLE_VIRTUAL_MEMORY QUERY AVAILABLE_VIRTUAL_MEMORY)
message(STATUS "AVAILABLE_VIRTUAL_MEMORY ==> ${AVAILABLE_VIRTUAL_MEMORY}")

cmake_host_system_information(RESULT TOTAL_PHYSICAL_MEMORY QUERY TOTAL_PHYSICAL_MEMORY)
message(STATUS "TOTAL_PHYSICAL_MEMORY ==> ${TOTAL_PHYSICAL_MEMORY}")

cmake_host_system_information(RESULT AVAILABLE_PHYSICAL_MEMORY QUERY AVAILABLE_PHYSICAL_MEMORY)
message(STATUS "AVAILABLE_PHYSICAL_MEMORY ==> ${AVAILABLE_PHYSICAL_MEMORY}")

cmake_host_system_information(RESULT IS_64BIT QUERY IS_64BIT)
message(STATUS "IS_64BIT ==> ${IS_64BIT}")

cmake_host_system_information(RESULT HAS_FPU QUERY HAS_FPU)
message(STATUS "HAS_FPU ==> ${HAS_FPU}")

cmake_host_system_information(RESULT HAS_MMX QUERY HAS_MMX)
message(STATUS "HAS_MMX ==> ${HAS_MMX}")

cmake_host_system_information(RESULT HAS_MMX_PLUS QUERY HAS_MMX_PLUS)
message(STATUS "HAS_MMX_PLUS ==> ${HAS_MMX_PLUS}")

cmake_host_system_information(RESULT HAS_SSE QUERY HAS_SSE)
message(STATUS "HAS_SSE ==> ${HAS_SSE}")

cmake_host_system_information(RESULT HAS_SSE2 QUERY HAS_SSE2)
message(STATUS "HAS_SSE2 ==> ${HAS_SSE2}")

cmake_host_system_information(RESULT HAS_SSE_FP QUERY HAS_SSE_FP)
message(STATUS "HAS_SSE_FP ==> ${HAS_SSE_FP}")

cmake_host_system_information(RESULT HAS_SSE_MMX QUERY HAS_SSE_MMX)
message(STATUS "HAS_SSE_MMX ==> ${HAS_SSE_MMX}")

cmake_host_system_information(RESULT HAS_AMD_3DNOW QUERY HAS_AMD_3DNOW)
message(STATUS "HAS_AMD_3DNOW ==> ${HAS_AMD_3DNOW}")

cmake_host_system_information(RESULT HAS_AMD_3DNOW_PLUS QUERY HAS_AMD_3DNOW_PLUS)
message(STATUS "HAS_AMD_3DNOW_PLUS ==> ${HAS_AMD_3DNOW_PLUS}")

cmake_host_system_information(RESULT HAS_IA64 QUERY HAS_IA64)
message(STATUS "HAS_IA64 ==> ${HAS_IA64}")

cmake_host_system_information(RESULT HAS_SERIAL_NUMBER QUERY HAS_SERIAL_NUMBER)
message(STATUS "HAS_SERIAL_NUMBER ==> ${HAS_SERIAL_NUMBER}")

cmake_host_system_information(RESULT PROCESSOR_SERIAL_NUMBER QUERY PROCESSOR_SERIAL_NUMBER)
message(STATUS "PROCESSOR_SERIAL_NUMBER ==> ${PROCESSOR_SERIAL_NUMBER}")

cmake_host_system_information(RESULT PROCESSOR_NAME QUERY PROCESSOR_NAME)
message(STATUS "PROCESSOR_NAME ==> ${PROCESSOR_NAME}")

cmake_host_system_information(RESULT PROCESSOR_DESCRIPTION QUERY PROCESSOR_DESCRIPTION)
message(STATUS "PROCESSOR_DESCRIPTION ==> ${PROCESSOR_DESCRIPTION}")

cmake_host_system_information(RESULT OS_NAME QUERY OS_NAME)
message(STATUS "OS_NAME ==> ${OS_NAME}")

cmake_host_system_information(RESULT OS_RELEASE QUERY OS_RELEASE)
message(STATUS "OS_RELEASE ==> ${OS_RELEASE}")

cmake_host_system_information(RESULT OS_VERSION QUERY OS_VERSION)
message(STATUS "OS_VERSION ==> ${OS_VERSION}")

cmake_host_system_information(RESULT OS_PLATFORM QUERY OS_PLATFORM)
message(STATUS "OS_PLATFORM ==> ${OS_PLATFORM}")

message(STATUS ===========================================)