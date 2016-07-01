Terraform AWS IAM Account Policy Module
===========

A Terraform module to set the account password policy within an AWS account

Input Variables
---------------

- `allow_users_to_change_password` - (Optional) To allow users to change their own password
- `hard_expiry` - (Optional) Users are prevented from setting a new password after their password has expired (i.e. require administrator reset)
- `max_password_age` - (Optional) The number of days that an user password is valid
- `minimum_password_length` - (Optional) Minimum length to require for user passwords
- `password_reuse_prevention` - (Optional) The number of previous passwords that users are prevented from reusing
- `require_lowercase_characters` - (Optional) To require lowercase characters for user passwords, default is true
- `require_numbers` - (Optional) To require numbers for user passwords, default is true
- `require_symbols` - (Optional) To require symbols for user passwords, default is false
- `require_uppercase_characters` - (Optional) To require uppercase characters for user passwords, default is true

Usage
-----


```module "my_iam_account_policy" {
  source = "github.com/mambetica/tf_aws_iam_account_policy"
}```