Module operator_csv_libs.tests.csv_test
=======================================

Classes
-------

`TestCSV(methodName='runTest')`
:   A class whose instances are single test cases.
    
    By default, the test code itself should be placed in a method named
    'runTest'.
    
    If the fixture may be used for many test cases, create as
    many test methods as are needed. When instantiating such a TestCase
    subclass, specify in the constructor arguments the name of the test method
    that the instance is to execute.
    
    Test authors should subclass TestCase for their own tests. Construction
    and deconstruction of the test's environment ('fixture') can be
    implemented by overriding the 'setUp' and 'tearDown' methods respectively.
    
    If it is necessary to override the __init__ method, the base class
    __init__ method must always be called. It is important that subclasses
    should not change the signature of their __init__ method, since instances
    of the classes are instantiated automatically by parts of the framework
    in order to be run.
    
    When subclassing TestCase, you can set these attributes:
    * failureException: determines which exception will be raised when
        the instance's assertion methods fail; test methods raising this
        exception will be deemed to have 'failed' rather than 'errored'.
    * longMessage: determines whether long messages (including repr of
        objects used in assert methods) will be printed on failure in *addition*
        to any explicit message passed.
    * maxDiff: sets the maximum length of a diff in failure messages
        by assert methods using difflib. It is looked up as an instance
        attribute so can be configured by individual tests if required.
    
    Create an instance of the class that will use the named test
    method when executed. Raises a ValueError if the instance does
    not have a method with the specified name.

    ### Ancestors (in MRO)

    * unittest.case.TestCase

    ### Methods

    `setUp(self)`
    :   Hook method for setting up the test fixture before exercising it.

    `test___update_operand_images(self)`
    :

    `test__get_deployments(self)`
    :

    `test__get_operator_images(self)`
    :

    `test__get_related_images(self)`
    :

    `test__setup_basic_logger(self)`
    :

    `test__update_operator_container_images(self)`
    :

    `test__update_version_references(self)`
    :

    `test_add_image_pullsecret(self)`
    :

    `test_generate_spec_relatedImages(self)`
    :

    `test_get_annotation_related_images(self)`
    :

    `test_get_operator_images(self)`
    :

    `test_get_owned_crds(self)`
    :

    `test_get_replaces(self)`
    :

    `test_get_updated_csv(self)`
    :

    `test_init(self)`
    :

    `test_set_deployments_annotations(self, key=None, value=None)`
    :

    `test_set_image_pullsecret(self)`
    :

    `test_set_replaces(self)`
    :

    `test_set_version(self)`
    :