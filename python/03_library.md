!SLIDE transition=none

# Lots Already Built #

 * Methods that use the shell (fabric)
  * fetch_
  * create_
  * assocate_

!SLIDE transition=none

# AMM #

 * publishing
 * users
 * pages

!SLIDE transition=none

# Members #

 * create members
 * login members
 * lists

!SLIDE transition=none

# Reg Blocks #

 * Fill in regblock with Lable/Value pairs
 * Any type of form field

!SLIDE transition=none

# ACE #

 * inventory
 * magic pages
 * scheduled tasks

!SLIDE transition=none

# APP #
 
 * reg blocks again
   * it's so nice to not have to constantly be filling out reg blocks.

!SLIDE smaller transition=none

    @@@python
    def fill_out_billing_info(self):

        email = self.get_unique_plus_email(
            self.config.as_str('email')
        )

        self.set_reg_block_field_by_label(
            'First Name', 'Selenium'
        )
        self.set_reg_block_field_by_label(
            'Last Name', 'Tester'
        )
        self.set_reg_block_field_by_label(
            'State', 'Minnesota'
        )
        self.set_reg_block_field_by_label(
            'Country', 'UNITED STATES'
        )

!SLIDE

# AMM Asserts #

 * `assert_valid_id(self, id)`
 * `assert_alert_and_accept(self)`
 * `assert_message(self, message)`
 * `assert_option_value_is_selected(self, select_element, value)`
 * `assert_option_label_is_selected(self, select_element, label)`
 * `assert_current_page_id(self, page_id)`
