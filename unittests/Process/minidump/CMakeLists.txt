add_lldb_unittest(LLDBMinidumpTests
  MinidumpParserTest.cpp
  )

set(test_inputs
   linux-i386.dmp
   linux-x86_64.dmp
   linux-x86_64_not_crashed.dmp
   fizzbuzz_no_heap.dmp
   fizzbuzz_wow64.dmp)

add_unittest_inputs(LLDBMinidumpTests "${test_inputs}")
