## Federal Information Processing Standards (FIPS)

| Acronym | Who made it | What is it | What does it mean? | Relevant standards | What makes us FIPS compliant? |
| ------- | ----------- | ---------- | ------------------ | -------| ---|
| FIPS | National Institute of Standards and Technology (NIST) | Set of standards vendors must adhere to when providing data processing services to US and Canadian govs | Product has been tested by ther Cryptographic module validation program (CMVP) and validated by NIST | [FIPS-140-2](https://csrc.nist.gov/pubs/fips/140-2/upd2/final) and [140-3 (newer standard)](https://csrc.nist.gov/pubs/fips/140-3/final) | FIPS images ship with validated redistribution of OpenSSL's FIPS provider module. Products using OpenSSL API can be converted to use FIPS-validated cryptography. We submitted a request for CMVP validation. For Java, we ship with FIPS variant of Bouncy Castle crypto package, Java implementation of cryptographic algorithms. 

## FedRAMP
- Requirement: use FIPS-validated cryptography