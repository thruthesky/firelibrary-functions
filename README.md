# firelibrary-functions
Google Cloud Functions For FireLibary

# TODO

* Produce error on thumbnailing with profile photo uploading and do proper error handling.


# install

* @see firelibrary readme

# known issues

* @see firelibrary readme



# Profile Photo

## Profile photo uploading.

1. client uploads => `data` class handles uploading.
2. `functions` creates thumbnail and updates user `profilePhoto` fields.
3. client listens on the profilePhoto fields and if there is update, update on profile update form.

## Profile photo deleting.

1. client deletes profile photo and its thumbnail and updates `profilePhoto` fields to empty.


## Profile photo updating/replacing.

1. client upload a new photo while old profile photo is being displayed(exists)

2. `data` class deletes old profile photo ( it does not update `profilePhoto` ) and its thumbnail
    and uploads new one.

3. `functions` creates thumbnail and updates user `profilePhoto`.




