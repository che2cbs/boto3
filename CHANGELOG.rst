Changelog
=========

Unreleased
----------

* feature:Resources: Make ``resource.meta`` a proper object. This allows
  you to do things like ``resource.meta.client``. This is a **backward-
  incompatible** change.
  (`issue 45 <https://github.com/boto/boto3/pull/45>`__)

0.0.6 - 2014-12-18
------------------

* feature:Amazon SQS: Add ``purge`` action to queue resources
* feature:Waiters: Add documentation for client and resource waiters
  (`issue 44 <https://github.com/boto/boto3/pull/44>`__)
* feature:Waiters: Add support for resource waiters
  (`issue 43 <https://github.com/boto/boto3/pull/43>`__)
* bugfix:Installation: Remove dependency on the unused ``six`` module
  (`issue 42 <https://github.com/boto/boto3/pull/42>`__)
* feature:Botocore: Update to Botocore 0.80.0

  * Update Amazon Simple Workflow Service (SWF) to the latest version
  * Update AWS Storage Gateway to the latest version
  * Update AWS Elastic MapReduce (EMR) to the latest version
  * Update AWS Elastic Transcoder to the latest version
  * Enable use of ``page_size`` for clients
    (`botocore issue 408 <https://github.com/boto/botocore/pull/408>`__)

0.0.5 - 2014-12-09
------------------

* feature: Add support for batch actions on collections.
  (`issue 32 <https://github.com/boto/boto3/pull/32>`__)
* feature: Update to Botocore 0.78.0

  * Add support for Amazon Simple Queue Service purge queue which allows
    users to delete the messages in their queue.
  * Add AWS OpsWorks support for registering and assigning existing Amazon
    EC2 instances and on-premises servers.
  * Fix issue with expired signatures when retrying failed requests
    (`botocore issue 399 <https://github.com/boto/botocore/pull/399>`__)
  * Port Route53 resource ID customizations from AWS CLI to Botocore.
    (`botocore issue 398 <https://github.com/boto/botocore/pull/398>`__)
  * Fix handling of blob type serialization for JSON services.
    (`botocore issue 397 <https://github.com/boto/botocore/pull/397>`__)

0.0.4 - 2014-12-04
------------------

* feature: Update to Botocore 0.77.0

  * Add support for Kinesis PutRecords operation. It writes multiple
    data records from a producer into an Amazon Kinesis stream in a
    single call.
  * Add support for IAM GetAccountAuthorizationDetails operation. It
    retrieves information about all IAM users, groups, and roles in
    your account, including their relationships to one another and
    their attached policies.
  * Add support for updating the comment of a Route53 hosted zone.
  * Fix base64 serialization for JSON protocol services.
  * Fix issue where certain timestamps were not being accepted as valid input
    (`botocore issue 389 <https://github.com/boto/botocore/pull/389>`__)

* feature: Update `Amazon EC2 <http://aws.amazon.com/ec2/>`_ resource model.
* feature: Support `belongsTo` resource reference as well as `path`
  specified in an action's resource definition.
* bugfix: Fix an issue accessing SQS message bodies
  (`issue 33 <https://github.com/boto/boto3/issues/33>`__)

0.0.3 - 2014-11-26
------------------

* feature: Update to Botocore 0.76.0.

  * Add support for using AWS Data Pipeline templates to create
    pipelines and bind values to parameters in the pipeline
  * Add support to Amazon Elastic Transcoder client for encryption of files
    in Amazon S3.
  * Fix issue where Amazon S3 requests were not being
    resigned correctly when using Signature Version 4.
    (`botocore issue 388 <https://github.com/boto/botocore/pull/388>`__)
  * Add support for custom response parsing in Botocore clients.
    (`botocore issue 387 <https://github.com/boto/botocore/pull/387>`__)

0.0.2 - 2014-11-20
------------------

* Adds resources for
  `AWS CloudFormation <http://aws.amazon.com/cloudformation/>`_ and
  `AWS OpsWorks <http://aws.amazon.com/opsworks/>`_.
* Update to Botocore 0.73.0 and JMESPath 0.5.0
* Adds support for
  `AWS CodeDeploy <http://aws.amazon.com/codedeploy/>`_,
  `AWS Config <http://aws.amazon.com/config/>`_,
  `AWS KMS <http://aws.amazon.com/kms/>`_,
  `AWS Lambda <http://aws.amazon.com/lambda/>`_.
* Make requests with a customized HTTP user-agent

0.0.1 - 2014-11-11
------------------

* Initial developer preview refresh of Boto 3
* Supports S3, EC2, SQS, SNS, and IAM resources
* Supports low-level clients for most services
