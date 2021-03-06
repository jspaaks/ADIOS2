#------------------------------------------------------------------------------#
# Distributed under the OSI-approved Apache License, Version 2.0.  See
# accompanying file Copyright.txt for details.
#------------------------------------------------------------------------------#

include(ADIOSFunctions)

if(ADIOS2_HAVE_MPI)
  gtest_add_tests_helper(Base TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscBase "" TRUE)

  gtest_add_tests_helper(OneSidedFencePush TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscOneSidedFencePush "" TRUE)

  gtest_add_tests_helper(OneSidedPostPush TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscOneSidedPostPush "" TRUE)

  gtest_add_tests_helper(OneSidedFencePull TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscOneSidedFencePull "" TRUE)

  gtest_add_tests_helper(OneSidedPostPull TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscOneSidedPostPull "" TRUE)

  gtest_add_tests_helper(Unbalanced TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscUnbalanced "" TRUE)

  gtest_add_tests_helper(WriterMultiblock TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscWriterMultiblock "" TRUE)

  gtest_add_tests_helper(ReaderMultiblock TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscReaderMultiblock "" TRUE)

  gtest_add_tests_helper(NoAttributes TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscNoAttributes "" TRUE)

  gtest_add_tests_helper(NoSelection TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscNoSelection "" TRUE)

  gtest_add_tests_helper(7d TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSsc7d "" TRUE)

  gtest_add_tests_helper(MoreReadersThanWriters TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscMoreReadersThanWriters "" TRUE)

  gtest_add_tests_helper(MoreWritersThanReaders TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscMoreWritersThanReaders "" TRUE)

  gtest_add_tests_helper(MultiApp TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscMultiApp "" TRUE)

  gtest_add_tests_helper(Xgc2Way TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscXgc2Way "" TRUE)

  gtest_add_tests_helper(Xgc3Way TRUE Ssc Engine.SSC. "")
  SetupTestPipeline(Engine.SSC.SscEngineTest.TestSscXgc3Way "" TRUE)

endif()
