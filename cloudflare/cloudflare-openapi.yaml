swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 1
info:
  title: CloudFlare
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/billing/subscriptions/apps:
    get:
      summary: List all of your app subscriptions
      description: List all of your app subscriptions
      operationId: cloudflare-app-subscription-api
      x-api-path-slug: userbillingsubscriptionsapps-get
      parameters:
      - in: query
        name: activated_on
        description: When the subscription was activated2014-03-01T12:20:00Z
      - in: query
        name: cancelled_on
        description: When the subscription was cancelled2014-04-01T12:20:00Z
      - in: query
        name: direction
        description: Direction to order subscriptionsdesc
      - in: query
        name: expired_on
        description: When the subscription expired2014-04-02T12:20:00Z
      - in: query
        name: expires_on
        description: When the subscription will expire2014-03-31T12:20:00Z
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: order
        description: Field to order subscriptions bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of items per page20
      - in: query
        name: price
        description: The price of the subscription that will be billed, in US dollars20
      - in: query
        name: renewed_on
        description: When the subscription was renewed2014-05-11T12:20:00Z
      - in: query
        name: status
        description: The state of the subscriptionactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /user/billing/subscriptions/apps/:identifier:
    get:
      summary: Billing subscription details
      description: Billing subscription details
      operationId: cloudflare-app-subscription-api
      x-api-path-slug: userbillingsubscriptionsappsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /zones/:zone_identifier/custom_pages:
    get:
      summary: A list of available Custom Pages the zone can use
      description: A list of available Custom Pages the zone can use
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pages-get
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/custom_pages/:identifier:
    get:
      summary: Details about a specific Custom page details
      description: Details about a specific Custom page details
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Zones
    put:
      summary: Update Custom page URL
      description: Update Custom page URL
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-put
      parameters:
      - in: query
        name: state
        description: The Custom Page statettttttttttttttdefault
      - in: query
        name: url
        description: A URL that is associated with the Custom Page
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/custom_certificates:
    get:
      summary: List, search, sort, and filter all of your custom SSL certificates
      description: List, search, sort, and filter all of your custom SSL certificates
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificates-get
      parameters:
      - in: query
        name: direction
        description: Direction to order zonesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: order
        description: Field to order certificates byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of zones per pagetttttttttttttt20
      - in: query
        name: status
        description: Status of the zones custom SSLttttttttttttttactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
    post:
      summary: Upload a new SSL certificate for a zone
      description: Upload a new SSL certificate for a zone
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificates-post
      parameters:
      - in: query
        name: certificate
        description: The zones SSL certificate or certificate and the intermediate(s)tttttttttttttt-----BEGIN
          CERTIFICATE----- MIIDtTCCAp2gAwIBAgIJAM15n7fdxhRtMA0GCSqGSIb3DQEBBQUAMEUxCzAJBgNV
          BAYTAlVTMRMwEQYDVQQIEwpTb21lLVN0YXRlMSEwHwYDVQQKExhJbnRlcm5ldCBX aWRnaXRzIFB0eSBMdGQwHhcNMTQwMzExMTkyMTU5WhcNMTQwNDEwMTkyMTU5WjBF
          MQswCQYDVQQGEwJVUzETMBEGA1UECBMKU29tZS1TdGF0ZTEhMB8GA1UEChMYSW50 ZXJuZXQgV2lkZ2l0cyBQdHkgTHRkMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
          CgKCAQEAvq3sKsHpeduJHimOK+fvQdKsI8z8A05MZyyLp2/R/GE8FjNv+hkVY1WQ LIyTNNQH7CJecE1nbTfo8Y56S7x/rhxC6/DJ8MIulapFPnorq46KU6yRxiM0MQ3N
          nTJHlHA2ozZta6YBBfVfhHWl1F0IfNbXCLKvGwWWMbCx43OfW6KTkbRnE6gFWKuO fSO5h2u5TaWVuSIzBvYs7Vza6m+gtYAvKAJV2nSZ+eSEFPDo29corOy8+huEOUL8
          5FAw4BFPsr1TlrlGPFitduQUHGrSL7skk1ESGza0to3bOtrodKei2s9bk5MXm7lZ qI+WZJX4Zu9+mzZhc9pCVi8r/qlXuQIDAQABo4GnMIGkMB0GA1UdDgQWBBRvavf+
          sWM4IwKiH9X9w1vl6nUVRDB1BgNVHSMEbjBsgBRvavf+sWM4IwKiH9X9w1vl6nUV RKFJpEcwRTELMAkGA1UEBhMCVVMxEzARBgNVBAgTClNvbWUtU3RhdGUxITAfBgNV
          BAoTGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZIIJAM15n7fdxhRtMAwGA1UdEwQF MAMBAf8wDQYJKoZIhvcNAQEFBQADggEBABY2ZzBaW0dMsAAT7tPJzrVWVzQx6KU4
          UEBLudIlWPlkAwTnINCWR/8eNjCCmGA4heUdHmazdpPa8RzwOmc0NT1NQqzSyktt vTqb4iHD7+8f9MqJ9/FssCfTtqr/Qst/hGH4Wmdf1EJ/6FqYAAb5iRlPgshFZxU8
          uXtA8hWn6fK6eISD9HBdcAFToUvKNZ1BIDPvh9f95Ine8ar6yGd56TUNrHR8eHBs ESxz5ddVR/oWRysNJ+aGAyYqHS8S/ttmC7r4XCAHqXptkHPCGRqkAhsterYhd4I8
          /cBzejUobNCjjHFbtkAL/SjxZOLW+pNkZwfeYdM8iPkD54Uua1v2tdw= -----END CERTIFICATE-----
      - in: query
        name: private_key
        description: The zones private keytttttttttttttt-----BEGIN RSA PRIVATE KEY-----MIIEowIBAAKCAQEAl
          1cSc0vfcJLI4ZdWjiZZqy86Eof4czCwilyjXdvHqbdgDjz9H6K/0FX78EzVdfyExESptPCDl5YYjvcZyAWlgNfYEpFpGeoh/pTFW3hlyKImh4EgBXbDrR251J
          Ew2Nf56X3duibI6X20gKZA6cvdmWeKh MOOXuh1bSPU3dkb4YOF/fng5iGrx0q3txdMQXTPMZ1uXHFcBH7idgViYesXUBhdll3GP1N
          Y8laq0yrqh 8HMsZK m27MebqonbNmjOqE218lVEvjCdRO6xvNXrO6vNJBoGn2eGwZ8BVd0mTA3Tj43/2cmxQFY9FLq56cCXqYI1fbRRib
          ZLrjSNkwIDAQABAoIBABfAjjsjjxc0NxcYvKOMUb9Rpj8Sx6U/o/tDC5u XmsGX37aaJmC5yw9BQiAxgvXtQryEl5uoNoqOdsxzKV6yM0vPcwKEJVBd4G6yx6AjVJZnc2qf72erR7BbA2CQh
          scMDRBKE041HhgTBRNP6roim0SOgYP5JZIrGAQXNIkyE0fZc5gZNUt388ne/mjWM6Xi08BDGurLC68nsdt7Nd
          UYqeBVxo2EqChp5vKYZYEcG8h9XBj4u4NIwg1Mty2JqX30uBjoHvF5w/pMs8lG uvj6JR9I
          19wtCuccbAJl 4cUq03UQoIDmwejea oC8A8WJr3vVpODDWrvAsjllGPBECgYEAyQRa6edYO6bsSvgbM13qXW9OQTn9YmgzfN24Ux1D66TQU6sBSLdfSHshDhTCi
          Ax 698aJNRWujAakA2DDgspSx98aRnHbF zvY7i7iWGesN6uN0zL 6/MK5uWoieGZRjgk230fLk00l4/FK1mJIp0apr0Lis9xmDjP5AaUPTUUCgYEAwXuhTHZWPT6v8YwOksjbuK
          UDkIIvyMux53kb73vrkgMboS4DB1zMLNyG 9EghS414CFROUwGl4ZUKboH1Jo5G34y8VgDuHjirTqL2H6
          zNpML iMrWCXjpFKkxwPbeQnEAZ 5Rud4d PTyXAt71blZHE9tZ4KHy8cU1iKc9APcCgYAIqKZd4vg7AZK2G//X85iv06aUSrIudfyZyVcyRVVyphPPNtOEVVnGXn9rAtvqeIrOo52BR68
          cj4vlXp hkDuEH QVBuY/NdQhOzFtPrKPQTJdGjIlQ2x65Vidj7r3sRukNkLPyV2v D885zcpTkp83JFuWTYiIrg275DIuAI3QKBgAglM0IrzS
          g3vlVQxvM1ussgRgkkYeybHq82 wUW 3DXLqeXb0s1DedplUkuoabZriz0Wh4GZFSmtA5ZpZC
          uV697lkYsndmp2xRhaekllW7bu pY5q88URwO2p8CO5AZ6CWFWuBwSDML5VOapGRqDRgwaD
          oGpb7fb7IgHOls7AoGBAJnL6Q8t35uYJ8J8hY7wso88IE04z6VaT8WganxcndesWER9eFQDHDDy//ZYeyt6M41uIY
          CL Vkm9Kwl/bHLJKdnOE1a9NdE6mtfah0Bk2u/YOuzyu5mmcgZiX X/OZuEbGmmbZOR1FCuIyrNYfwYohhcZP7/r0Ia/1GpkHc3Bi-----END
          RSA PRIVATE KEY-----
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /zones/:zone_identifier/custom_certificates/:identifier:
    delete:
      summary: 'Delete an SSL certificate permission needed: #ssl:edit'
      description: 'Delete an SSL certificate permission needed: #ssl:editntt'
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Certificates
    get:
      summary: 'SSL configuration details permission needed: #ssl:read'
      description: 'SSL configuration details permission needed: #ssl:readntt'
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Certificates
    patch:
      summary: Upload a new private key and/or PEM/CRT for the SSL certificate
      description: Upload a new private key and/or PEM/CRT for the SSL certificate
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-patch
      parameters:
      - in: query
        name: certificate
        description: The zones SSL certificate or certificate and the intermediate(s)tttttttttttttt-----BEGIN
          CERTIFICATE----- MIIDtTCCAp2gAwIBAgIJAM15n7fdxhRtMA0GCSqGSIb3DQEBBQUAMEUxCzAJBgNV
          BAYTAlVTMRMwEQYDVQQIEwpTb21lLVN0YXRlMSEwHwYDVQQKExhJbnRlcm5ldCBX aWRnaXRzIFB0eSBMdGQwHhcNMTQwMzExMTkyMTU5WhcNMTQwNDEwMTkyMTU5WjBF
          MQswCQYDVQQGEwJVUzETMBEGA1UECBMKU29tZS1TdGF0ZTEhMB8GA1UEChMYSW50 ZXJuZXQgV2lkZ2l0cyBQdHkgTHRkMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
          CgKCAQEAvq3sKsHpeduJHimOK+fvQdKsI8z8A05MZyyLp2/R/GE8FjNv+hkVY1WQ LIyTNNQH7CJecE1nbTfo8Y56S7x/rhxC6/DJ8MIulapFPnorq46KU6yRxiM0MQ3N
          nTJHlHA2ozZta6YBBfVfhHWl1F0IfNbXCLKvGwWWMbCx43OfW6KTkbRnE6gFWKuO fSO5h2u5TaWVuSIzBvYs7Vza6m+gtYAvKAJV2nSZ+eSEFPDo29corOy8+huEOUL8
          5FAw4BFPsr1TlrlGPFitduQUHGrSL7skk1ESGza0to3bOtrodKei2s9bk5MXm7lZ qI+WZJX4Zu9+mzZhc9pCVi8r/qlXuQIDAQABo4GnMIGkMB0GA1UdDgQWBBRvavf+
          sWM4IwKiH9X9w1vl6nUVRDB1BgNVHSMEbjBsgBRvavf+sWM4IwKiH9X9w1vl6nUV RKFJpEcwRTELMAkGA1UEBhMCVVMxEzARBgNVBAgTClNvbWUtU3RhdGUxITAfBgNV
          BAoTGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZIIJAM15n7fdxhRtMAwGA1UdEwQF MAMBAf8wDQYJKoZIhvcNAQEFBQADggEBABY2ZzBaW0dMsAAT7tPJzrVWVzQx6KU4
          UEBLudIlWPlkAwTnINCWR/8eNjCCmGA4heUdHmazdpPa8RzwOmc0NT1NQqzSyktt vTqb4iHD7+8f9MqJ9/FssCfTtqr/Qst/hGH4Wmdf1EJ/6FqYAAb5iRlPgshFZxU8
          uXtA8hWn6fK6eISD9HBdcAFToUvKNZ1BIDPvh9f95Ine8ar6yGd56TUNrHR8eHBs ESxz5ddVR/oWRysNJ+aGAyYqHS8S/ttmC7r4XCAHqXptkHPCGRqkAhsterYhd4I8
          /cBzejUobNCjjHFbtkAL/SjxZOLW+pNkZwfeYdM8iPkD54Uua1v2tdw= -----END CERTIFICATE-----
      - in: query
        name: private_key
        description: The zones private keytttttttttttttt-----BEGIN RSA PRIVATE KEY-----MIIEowIBAAKCAQEAl
          1cSc0vfcJLI4ZdWjiZZqy86Eof4czCwilyjXdvHqbdgDjz9H6K/0FX78EzVdfyExESptPCDl5YYjvcZyAWlgNfYEpFpGeoh/pTFW3hlyKImh4EgBXbDrR251J
          Ew2Nf56X3duibI6X20gKZA6cvdmWeKh MOOXuh1bSPU3dkb4YOF/fng5iGrx0q3txdMQXTPMZ1uXHFcBH7idgViYesXUBhdll3GP1N
          Y8laq0yrqh 8HMsZK m27MebqonbNmjOqE218lVEvjCdRO6xvNXrO6vNJBoGn2eGwZ8BVd0mTA3Tj43/2cmxQFY9FLq56cCXqYI1fbRRib
          ZLrjSNkwIDAQABAoIBABfAjjsjjxc0NxcYvKOMUb9Rpj8Sx6U/o/tDC5u XmsGX37aaJmC5yw9BQiAxgvXtQryEl5uoNoqOdsxzKV6yM0vPcwKEJVBd4G6yx6AjVJZnc2qf72erR7BbA2CQh
          scMDRBKE041HhgTBRNP6roim0SOgYP5JZIrGAQXNIkyE0fZc5gZNUt388ne/mjWM6Xi08BDGurLC68nsdt7Nd
          UYqeBVxo2EqChp5vKYZYEcG8h9XBj4u4NIwg1Mty2JqX30uBjoHvF5w/pMs8lG uvj6JR9I
          19wtCuccbAJl 4cUq03UQoIDmwejea oC8A8WJr3vVpODDWrvAsjllGPBECgYEAyQRa6edYO6bsSvgbM13qXW9OQTn9YmgzfN24Ux1D66TQU6sBSLdfSHshDhTCi
          Ax 698aJNRWujAakA2DDgspSx98aRnHbF zvY7i7iWGesN6uN0zL 6/MK5uWoieGZRjgk230fLk00l4/FK1mJIp0apr0Lis9xmDjP5AaUPTUUCgYEAwXuhTHZWPT6v8YwOksjbuK
          UDkIIvyMux53kb73vrkgMboS4DB1zMLNyG 9EghS414CFROUwGl4ZUKboH1Jo5G34y8VgDuHjirTqL2H6
          zNpML iMrWCXjpFKkxwPbeQnEAZ 5Rud4d PTyXAt71blZHE9tZ4KHy8cU1iKc9APcCgYAIqKZd4vg7AZK2G//X85iv06aUSrIudfyZyVcyRVVyphPPNtOEVVnGXn9rAtvqeIrOo52BR68
          cj4vlXp hkDuEH QVBuY/NdQhOzFtPrKPQTJdGjIlQ2x65Vidj7r3sRukNkLPyV2v D885zcpTkp83JFuWTYiIrg275DIuAI3QKBgAglM0IrzS
          g3vlVQxvM1ussgRgkkYeybHq82 wUW 3DXLqeXb0s1DedplUkuoabZriz0Wh4GZFSmtA5ZpZC
          uV697lkYsndmp2xRhaekllW7bu pY5q88URwO2p8CO5AZ6CWFWuBwSDML5VOapGRqDRgwaD
          oGpb7fb7IgHOls7AoGBAJnL6Q8t35uYJ8J8hY7wso88IE04z6VaT8WganxcndesWER9eFQDHDDy//ZYeyt6M41uIY
          CL Vkm9Kwl/bHLJKdnOE1a9NdE6mtfah0Bk2u/YOuzyu5mmcgZiX X/OZuEbGmmbZOR1FCuIyrNYfwYohhcZP7/r0Ia/1GpkHc3Bi-----END
          RSA PRIVATE KEY-----
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /zones/:zone_identifier/custom_certificates/prioritize:
    put:
      summary: If a zone has multiple SSL certificates, you can set the order in which
        they should be used during a request
      description: If a zone has multiple SSL certificates, you can set the order
        in which they should be used during a request
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesprioritize-put
      parameters:
      - in: query
        name: certificates
        description: Array of ordered certificates
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /zones/:zone_identifier/dns_records:
    get:
      summary: List, search, sort, and filter a zones&#39; DNS records
      description: List, search, sort, and filter a zones&#39; DNS records
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-records-get
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: direction
        description: Direction to order domainsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: order
        description: Field to order records bytttttttttttttttype
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of DNS records per pagetttttttttttttt20
      - in: query
        name: type
        description: DNS record typettttttttttttttA
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Records
    post:
      summary: Create a new DNS record for a zone
      description: Create a new DNS record for a zone
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-records-post
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: type
        description: DNS record typettttttttttttttA
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Records
  /zones/:zone_identifier/dns_records/:identifier:
    delete:
      summary: 'Delete DNS record permission needed: #dns_records:edit'
      description: 'Delete DNS record permission needed: #dns_records:editntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Records
    get:
      summary: 'DNS record details permission needed: #dns_records:read'
      description: 'DNS record details permission needed: #dns_records:readntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Records
    put:
      summary: 'Update DNS record permission needed: #dns_records:edit'
      description: 'Update DNS record permission needed: #dns_records:editntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-put
      responses:
        200:
          description: OK
      tags:
      - Records
  /zones/:zone_id/firewall/access_rules/rules:
    get:
      summary: Search, sort, and filter IP/country access rules
      description: Search, sort, and filter IP/country access rules
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      x-api-path-slug: zoneszone-idfirewallaccess-rulesrules-get
      parameters:
      - in: query
        name: configuration_target
        description: The rule configuration targetttttttttttttttip
      - in: query
        name: configuration_value
        description: Search by IP, range, or country codetttttttttttttt1
      - in: query
        name: direction
        description: Direction to order rulesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: order
        description: Field to order rules byttttttttttttttscope_type
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of rules per pagetttttttttttttt50
      - in: query
        name: scope_type
        description: The scope of the rulesttttttttttttttzone
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Firewall Access Rule
    post:
      summary: Make a new IP, IP range, or country access rule for the zone
      description: Make a new IP, IP range, or country access rule for the zone
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      x-api-path-slug: zoneszone-idfirewallaccess-rulesrules-post
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Firewall Access Rule
  /zones/:zone_id/firewall/access_rules/rules/:identifier:
    delete:
      summary: Remove an access rule so it is no longer evaluated during requests
      description: Remove an access rule so it is no longer evaluated during requests
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      x-api-path-slug: zoneszone-idfirewallaccess-rulesrulesidentifier-delete
      parameters:
      - in: query
        name: cascade
        description: The level to attempt to delete rules defined on other zones that
          are similar to this rulettttttttttttttnone
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Firewall Access Rule
    patch:
      summary: Update rule state and/or configuration for the zone
      description: Update rule state and/or configuration for the zone
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      x-api-path-slug: zoneszone-idfirewallaccess-rulesrulesidentifier-patch
      parameters:
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: notes
        description: A personal note about the rule
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Firewall Access Rule
  /zones/:zone_identifier/keyless_certificates:
    get:
      summary: List all Keyless SSL configurations for a given zone
      description: List all Keyless SSL configurations for a given zone
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifierkeyless-certificates-get
      responses:
        200:
          description: OK
      tags:
      - Keyless Certificates
    post:
      summary: The keyless SSL name
      description: The keyless SSL name
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifierkeyless-certificates-post
      parameters:
      - in: query
        name: certificate
        description: The zones SSL certificate or SSL certificate and intermediate(s)tttttttttttttt-----BEGIN
          CERTIFICATE----- MIIDtTCCAp2gAwIBAgIJAM15n7fdxhRtMA0GCSqGSIb3DQEBBQUAMEUxCzAJBgNV
          BAYTAlVTMRMwEQYDVQQIEwpTb21lLVN0YXRlMSEwHwYDVQQKExhJbnRlcm5ldCBX aWRnaXRzIFB0eSBMdGQwHhcNMTQwMzExMTkyMTU5WhcNMTQwNDEwMTkyMTU5WjBF
          MQswCQYDVQQGEwJVUzETMBEGA1UECBMKU29tZS1TdGF0ZTEhMB8GA1UEChMYSW50 ZXJuZXQgV2lkZ2l0cyBQdHkgTHRkMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
          CgKCAQEAvq3sKsHpeduJHimOK+fvQdKsI8z8A05MZyyLp2/R/GE8FjNv+hkVY1WQ LIyTNNQH7CJecE1nbTfo8Y56S7x/rhxC6/DJ8MIulapFPnorq46KU6yRxiM0MQ3N
          nTJHlHA2ozZta6YBBfVfhHWl1F0IfNbXCLKvGwWWMbCx43OfW6KTkbRnE6gFWKuO fSO5h2u5TaWVuSIzBvYs7Vza6m+gtYAvKAJV2nSZ+eSEFPDo29corOy8+huEOUL8
          5FAw4BFPsr1TlrlGPFitduQUHGrSL7skk1ESGza0to3bOtrodKei2s9bk5MXm7lZ qI+WZJX4Zu9+mzZhc9pCVi8r/qlXuQIDAQABo4GnMIGkMB0GA1UdDgQWBBRvavf+
          sWM4IwKiH9X9w1vl6nUVRDB1BgNVHSMEbjBsgBRvavf+sWM4IwKiH9X9w1vl6nUV RKFJpEcwRTELMAkGA1UEBhMCVVMxEzARBgNVBAgTClNvbWUtU3RhdGUxITAfBgNV
          BAoTGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZIIJAM15n7fdxhRtMAwGA1UdEwQF MAMBAf8wDQYJKoZIhvcNAQEFBQADggEBABY2ZzBaW0dMsAAT7tPJzrVWVzQx6KU4
          UEBLudIlWPlkAwTnINCWR/8eNjCCmGA4heUdHmazdpPa8RzwOmc0NT1NQqzSyktt vTqb4iHD7+8f9MqJ9/FssCfTtqr/Qst/hGH4Wmdf1EJ/6FqYAAb5iRlPgshFZxU8
          uXtA8hWn6fK6eISD9HBdcAFToUvKNZ1BIDPvh9f95Ine8ar6yGd56TUNrHR8eHBs ESxz5ddVR/oWRysNJ+aGAyYqHS8S/ttmC7r4XCAHqXptkHPCGRqkAhsterYhd4I8
          /cBzejUobNCjjHFbtkAL/SjxZOLW+pNkZwfeYdM8iPkD54Uua1v2tdw= -----END CERTIFICATE-----
      - in: query
        name: host
        description: The keyless SSL namettttttttttttttexample
      - in: query
        name: name
        description: The keyless SSL namettttttttttttttexample
      - in: query
        name: port
        description: The keyless SSL port used to commmunicate between CloudFlare
          and the clients Keyless SSL servertttttttttttttt24008
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Keyless Certificates
  /zones/:zone_identifier/keyless_certificates/:identifier:
    delete:
      summary: 'Delete Keyless configuration permission needed: #ssl:edit'
      description: 'Delete Keyless configuration permission needed: #ssl:editntt'
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifierkeyless-certificatesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Keyless Certificates
    get:
      summary: Details for one Keyless SSL configuration
      description: Details for one Keyless SSL configuration
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifierkeyless-certificatesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Keyless Certificates
    patch:
      summary: This will update attributes of a Keyless SSL
      description: This will update attributes of a Keyless SSL
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifierkeyless-certificatesidentifier-patch
      parameters:
      - in: query
        name: host
        description: The keyless SSL namettttttttttttttexample
      - in: query
        name: name
        description: The keyless SSL namettttttttttttttexample
      - in: query
        name: port
        description: The keyless SSL port used to commmunicate between CloudFlare
          and the clients Keyless SSL servertttttttttttttt24008
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Keyless Certificates
  /organizations/:organization_identifier/invite/:identifier:
    patch:
      summary: Change the Roles of a Pending Invite
      description: Change the Roles of a Pending Invite
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinviteidentifier-patch
      parameters:
      - in: query
        name: roles
        description: Array of Roles associated with the invited usertttttttttttttt[3536bcfad5faccb999b47003c79917fb]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/invites:
    get:
      summary: List all invitations associated with an organization
      description: List all invitations associated with an organization
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvites-get
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
    post:
      summary: Invite a User to become a Member of an Organization
      description: Invite a User to become a Member of an Organization
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvites-post
      parameters:
      - in: query
        name: invited_member_email
        description: Email address of the user to be added to the Organizationttttttttttttttuser@example
      - in: query
        name: roles
        description: Array of Roles associated with the invited usertttttttttttttt[{id:5a7805061c76ada191ed06f989cc3dac},{id:9a7806061c88ada191ed06f989cc3dac}]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/invites/:identifier:
    delete:
      summary: Cancel an existing invitation
      description: Cancel an existing invitation
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvitesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
    get:
      summary: Get the details of an invitation
      description: Get the details of an invitation
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvitesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/members:
    get:
      summary: List all members of a organization
      description: List all members of a organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembers-get
      responses:
        200:
          description: OK
      tags:
      - Organization Members
  /organizations/:organization_identifier/members/:identifier:
    delete:
      summary: Remove a member from an organization
      description: Remove a member from an organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Members
    get:
      summary: Get information about a specific member of an organization
      description: Get information about a specific member of an organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Members
    patch:
      summary: Change the Roles of an Organization&#39;s Member
      description: Change the Roles of an Organization&#39;s Member
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-patch
      parameters:
      - in: query
        name: roles
        description: Array of Roles associated with this Membertttttttttttttt[3536bcfad5faccb999b47003c79917fb]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Members
  /organizations/:organization_identifier/roles:
    get:
      summary: Get all available roles for an organization
      description: Get all available roles for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierroles-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
  /organizations/:organization_identifier/roles/:identifier:
    get:
      summary: Get information about a specific role for an organization
      description: Get information about a specific role for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierrolesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
  /organizations/:organization_id/firewall/access_rules/rules:
    get:
      summary: Search, sort, and filter IP/country access rules
      description: Search, sort, and filter IP/country access rules
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrules-get
      parameters:
      - in: query
        name: configuration_target
        description: The rule configuration targetttttttttttttttip
      - in: query
        name: configuration_value
        description: Search by IP, range, or country codetttttttttttttt1
      - in: query
        name: direction
        description: Direction to order rulesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: order
        description: Field to order rules byttttttttttttttmode
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of rules per pagetttttttttttttt50
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
    post:
      summary: Make a new IP, IP range, or country access rule for all zones owned
        by the organization
      description: Make a new IP, IP range, or country access rule for all zones owned
        by the organization
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrules-post
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
  /organizations/:organization_id/firewall/access_rules/rules/:identifier:
    delete:
      summary: Remove an access rule so it is no longer evaluated during requests
      description: Remove an access rule so it is no longer evaluated during requests
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrulesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
    patch:
      summary: Update rule state and/or configuration
      description: Update rule state and/or configuration
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrulesidentifier-patch
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
  /organizations/:identifier:
    get:
      summary: Get information about a specific organization that you are a member
        of
      description: Get information about a specific organization that you are a member
        of
      operationId: cloudflare-organizations-api
      x-api-path-slug: organizationsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    patch:
      summary: Update an existing Organization
      description: Update an existing Organization
      operationId: cloudflare-organizations-api
      x-api-path-slug: organizationsidentifier-patch
      parameters:
      - in: query
        name: name
        description: Organization NamettttttttttttttCloudFlare, Inc
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /railguns:
    get:
      summary: List, search, sort and filter your Railguns
      description: List, search, sort and filter your Railguns
      operationId: cloudflare-railgun-api
      x-api-path-slug: railguns-get
      parameters:
      - in: query
        name: direction
        description: Direction to order Railgunsttttttttttttttdesc
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of items per pagetttttttttttttt20
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Performance
    post:
      summary: Readable identifier of the railgun
      description: Readable identifier of the railgun
      operationId: cloudflare-railgun-api
      x-api-path-slug: railguns-post
      parameters:
      - in: query
        name: name
        description: Readable identifier of the railgunttttttttttttttMy Railgun
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Performance
  /railguns/:identifier:
    delete:
      summary: Disable and delete a Railgun
      description: Disable and delete a Railgun
      operationId: cloudflare-railgun-api
      x-api-path-slug: railgunsidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Performance
    get:
      summary: Railgun details
      description: Railgun detailsntt
      operationId: cloudflare-railgun-api
      x-api-path-slug: railgunsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Performance
    patch:
      summary: Enable or disable a Railgun for all zones connected to it
      description: Enable or disable a Railgun for all zones connected to it
      operationId: cloudflare-railgun-api
      x-api-path-slug: railgunsidentifier-patch
      parameters:
      - in: query
        name: enabled
        description: Flag to determine if the Railgun is accepting connectionstttttttttttttttrue
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Performance
  /railguns/:identifier/zones:
    get:
      summary: The zones that are currently using this Railgun
      description: The zones that are currently using this Railgun
      operationId: cloudflare-railgun-api
      x-api-path-slug: railgunsidentifierzones-get
      responses:
        200:
          description: OK
      tags:
      - Performance
  /zones/:zone_identifier/railguns:
    get:
      summary: A list of available Railguns the zone can use
      description: A list of available Railguns the zone can use
      operationId: cloudflare-railgun-connections-for-a-zone-api
      x-api-path-slug: zoneszone-identifierrailguns-get
      responses:
        200:
          description: OK
      tags:
      - Performance
  /zones/:zone_identifier/railguns/:identifier:
    get:
      summary: Details about a specific Railgun
      description: Details about a specific Railgun
      operationId: cloudflare-railgun-connections-for-a-zone-api
      x-api-path-slug: zoneszone-identifierrailgunsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Performance
    patch:
      summary: Connect or disconnect a Railgun
      description: Connect or disconnect a Railgun
      operationId: cloudflare-railgun-connections-for-a-zone-api
      x-api-path-slug: zoneszone-identifierrailgunsidentifier-patch
      parameters:
      - in: query
        name: connected
        description: A flag indicating whether the given zone is connected to the
          Railguntttttttttttttttrue
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Performance
  /zones/:zone_identifier/railguns/:identifier/diagnose:
    get:
      summary: Test Railgun connection to the Zone
      description: Test Railgun connection to the Zone
      operationId: cloudflare-railgun-connections-for-a-zone-api
      x-api-path-slug: zoneszone-identifierrailgunsidentifierdiagnose-get
      responses:
        200:
          description: OK
      tags:
      - Performance
  /user:
    get:
      summary: User details
      description: User detailsn
      operationId: cloudflare-user-api
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Update part of your user details
      description: Update part of your user details
      operationId: cloudflare-user-api
      x-api-path-slug: user-patch
      parameters:
      - in: query
        name: country
        description: The country in which the user lives
      - in: query
        name: first_name
        description: Users first nameJohn
      - in: query
        name: last_name
        description: Users last nameAppleseed
      - in: query
        name: telephone
        description: Users telephone number+1 123-123-1234
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      - in: query
        name: zipcode
        description: The zipcode or postal code where the user lives
      responses:
        200:
          description: OK
      tags:
      - Users
  /user/billing/history:
    get:
      summary: Access your billing history object
      description: Access your billing history object
      operationId: cloudflare-user-billing-history-api
      x-api-path-slug: userbillinghistory-get
      parameters:
      - in: query
        name: action
        description: The billing item actionsubscription
      - in: query
        name: occured_at
        description: When the billing item was created2014-03-01T12:21:59
      - in: query
        name: order
        description: Field to order billing history byoccured_at
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of items per page20
      - in: query
        name: type
        description: The billing item typecharge
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Billing History
  /user/billing/profile:
    get:
      summary: Access your billing profile object
      description: Access your billing profile object
      operationId: cloudflare-user-billing-profile-api
      x-api-path-slug: userbillingprofile-get
      responses:
        200:
          description: OK
      tags:
      - Billing Profile
  /user/firewall/access_rules/rules:
    get:
      summary: Search, sort, and filter IP/country access rules
      description: Search, sort, and filter IP/country access rules
      operationId: cloudflare-userlevel-firewall-access-rule-api
      x-api-path-slug: userfirewallaccess-rulesrules-get
      parameters:
      - in: query
        name: configuration_target
        description: The rule configuration targetip
      - in: query
        name: configuration_value
        description: Search by IP, range, or country code1
      - in: query
        name: direction
        description: Direction to order rulesdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: mode
        description: The action to apply to a matched requestchallenge
      - in: query
        name: order
        description: Field to order rules bymode
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of rules per page50
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Level Firewall Access Rule
    post:
      summary: Make a new IP, IP range, or country access rule for all zones owned
        by the user
      description: Make a new IP, IP range, or country access rule for all zones owned
        by the user
      operationId: cloudflare-userlevel-firewall-access-rule-api
      x-api-path-slug: userfirewallaccess-rulesrules-post
      parameters:
      - in: query
        name: configuration
        description: Rule configurationOne of the following:Show definition &raquo;Name
          /typeDescription /exampleConstraintstargetstring
      - in: query
        name: mode
        description: The action to apply to a matched requestchallenge
      - in: query
        name: value
        description: The IP address to target in requests1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Level Firewall Access Rule
  /user/firewall/access_rules/rules/:identifier:
    delete:
      summary: Remove an access rule so it is no longer evaluated during requests
      description: Remove an access rule so it is no longer evaluated during requests
      operationId: cloudflare-userlevel-firewall-access-rule-api
      x-api-path-slug: userfirewallaccess-rulesrulesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - User Level Firewall Access Rule
    patch:
      summary: Update rule state and/or configuration
      description: Update rule state and/or configuration
      operationId: cloudflare-userlevel-firewall-access-rule-api
      x-api-path-slug: userfirewallaccess-rulesrulesidentifier-patch
      parameters:
      - in: query
        name: configuration
        description: Rule configurationOne of the following:Show definition &raquo;Name
          /typeDescription /exampleConstraintstargetstring
      - in: query
        name: mode
        description: The action to apply to a matched requestchallenge
      - in: query
        name: value
        description: The IP address to target in requests1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Level Firewall Access Rule
  /user/invites:
    get:
      summary: List all invitations associated with my user
      description: List all invitations associated with my user
      operationId: cloudflare-userx27s-invites-api
      x-api-path-slug: userinvites-get
      responses:
        200:
          description: OK
      tags:
      - User Invites
  /user/invites/:identifier:
    get:
      summary: Get the details of an invitation
      description: Get the details of an invitation
      operationId: cloudflare-userx27s-invites-api
      x-api-path-slug: userinvitesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - User Invites
    patch:
      summary: Respond to an invitation
      description: Respond to an invitation
      operationId: cloudflare-userx27s-invites-api
      x-api-path-slug: userinvitesidentifier-patch
      parameters:
      - in: query
        name: status
        description: Status of your response to the invitation (rejected or accepted)accepted
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Invites
  /user/organizations:
    get:
      summary: List organizations the user is associated with
      description: List organizations the user is associated with
      operationId: cloudflare-userx27s-organizations-api
      x-api-path-slug: userorganizations-get
      parameters:
      - in: query
        name: direction
        description: Direction to order organizationsdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: name
        description: Organization NameCloudFlare, Inc
      - in: query
        name: order
        description: Field to order organizations bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of organizations per page20
      - in: query
        name: status
        description: Whether or not the user is a member of the organization or has
          an inivitation pendingmember
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - User Organizations
  /user/organizations/:identifier:
    delete:
      summary: Remove association to an organization
      description: Remove association to an organization
      operationId: cloudflare-userx27s-organizations-api
      x-api-path-slug: userorganizationsidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - User Organizations
    get:
      summary: Get a specific organization the user is associated with
      description: Get a specific organization the user is associated with
      operationId: cloudflare-userx27s-organizations-api
      x-api-path-slug: userorganizationsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - User Organizations
  /zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups:
    get:
      summary: Search, list, and sort rule groups contained within a package
      description: Search, list, and sort rule groups contained within a package
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroups-get
      parameters:
      - in: query
        name: direction
        description: Direction to order groupsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: Whether or not the rules contained within this group are configurable/usabletttttttttttttton
      - in: query
        name: name
        description: Name of the firewall rule groupttttttttttttttProject Honey Pot
      - in: query
        name: order
        description: Field to order groups byttttttttttttttmode
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of groups per pagetttttttttttttt50
      - in: query
        name: rules_count
        description: How many rules are contained within this grouptttttttttttttt10
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
  /zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier:
    get:
      summary: Get a single rule group
      description: Get a single rule group
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
    patch:
      summary: Update the state of a rule group
      description: Update the state of a rule group
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-patch
      parameters:
      - in: query
        name: mode
        description: Whether or not the rules contained within this group are configurable/usabletttttttttttttton
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
  /zones/:zone_identifier/firewall/waf/packages:
    get:
      summary: Retrieve firewall packages for a zone
      description: Retrieve firewall packages for a zone
      operationId: cloudflare-waf-rule-packages-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackages-get
      parameters:
      - in: query
        name: direction
        description: Direction to order packagesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: Name of the firewall packagettttttttttttttWordPress rules
      - in: query
        name: order
        description: Field to order packages byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of packages per pagetttttttttttttt50
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Packages
  /zones/:zone_identifier/firewall/waf/packages/:identifier:
    get:
      summary: Get information about a single firewall package
      description: Get information about a single firewall package
      operationId: cloudflare-waf-rule-packages-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Packages
    patch:
      summary: Change the sensitivity and action for an anomaly detection type WAF
        rule package
      description: Change the sensitivity and action for an anomaly detection type
        WAF rule package
      operationId: cloudflare-waf-rule-packages-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagesidentifier-patch
      parameters:
      - in: query
        name: action_mode
        description: The default action that will be taken for rules under the firewall
          package
      - in: query
        name: sensitivity
        description: The sensitivity of the firewall package
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Packages
  /zones/:zone_id/firewall/waf/packages/:package_id/rules:
    get:
      summary: Search, sort, and filter rules within a package
      description: Search, sort, and filter rules within a package
      operationId: cloudflare-waf-rules-api
      x-api-path-slug: zoneszone-idfirewallwafpackagespackage-idrules-get
      parameters:
      - in: query
        name: description
        description: Public description of the rulettttttttttttttSQL injection prevention
          for SELECT statements
      - in: query
        name: direction
        description: Direction to order rulesttttttttttttttdesc
      - in: query
        name: group_id
        description: WAF group identifier tagttttttttttttttde677e5818985db1285d0e80225f06e5
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: The rule modetttttttttttttttttttttOne of the following:ttttttttttttttttttttttWhether
          or not the anomaly-based rule will be used when evaluating the request
      - in: query
        name: order
        description: Field to order rules byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of rules per pagetttttttttttttt50
      - in: query
        name: priority
        description: The order in which the individual rule is executed within the
          related grouptttttttttttttt5
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rules
  /zones/:zone_id/firewall/waf/packages/:package_id/rules/:identifier:
    get:
      summary: Individual information about a rule
      description: Individual information about a rule
      operationId: cloudflare-waf-rules-api
      x-api-path-slug: zoneszone-idfirewallwafpackagespackage-idrulesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - WAF Rules
    patch:
      summary: Update the action the rule will perform if triggered on the zone
      description: Update the action the rule will perform if triggered on the zone
      operationId: cloudflare-waf-rules-api
      x-api-path-slug: zoneszone-idfirewallwafpackagespackage-idrulesidentifier-patch
      parameters:
      - in: query
        name: mode
        description: The mode to use when the rule is triggered
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rules
  /zones/:zone_identifier/analytics/colos:
    get:
      summary: This view provides a breakdown of analytics data by datacenter
      description: This view provides a breakdown of analytics data by datacenter
      operationId: cloudflare-zone-analytics-api
      x-api-path-slug: zoneszone-identifieranalyticscolos-get
      parameters:
      - in: query
        name: continuous
        description: When set to true, the range returned by the response acts like
          a sliding window to provide a contiguous time-window
      - in: query
        name: since
        description: The (inclusive) beginning of the requested time frame
      - in: query
        name: until
        description: The (exclusive) end of the requested time frame
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Analytics
  /zones/:zone_identifier/analytics/dashboard:
    get:
      summary: The dashboard view provides both totals and timeseries data for the
        given zone and time period across the entire CloudFlare network
      description: The dashboard view provides both totals and timeseries data for
        the given zone and time period across the entire CloudFlare network
      operationId: cloudflare-zone-analytics-api
      x-api-path-slug: zoneszone-identifieranalyticsdashboard-get
      parameters:
      - in: query
        name: continuous
        description: When set to true, the range returned by the response acts like
          a sliding window to provide a contiguous time-window
      - in: query
        name: since
        description: The (inclusive) beginning of the requested time frame
      - in: query
        name: until
        description: The (exclusive) end of the requested time frame
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Analytics
  /zones:
    get:
      summary: List, search, sort, and filter your zones
      description: List, search, sort, and filter your zones
      operationId: cloudflare-zone-api
      x-api-path-slug: zones-get
      parameters:
      - in: query
        name: direction
        description: Direction to order zonesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: A domain namettttttttttttttexample
      - in: query
        name: order
        description: Field to order zones byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of zones per pagetttttttttttttt20
      - in: query
        name: status
        description: Status of the zonettttttttttttttactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
    post:
      summary: The domain name
      description: The domain name
      operationId: cloudflare-zone-api
      x-api-path-slug: zones-post
      parameters:
      - in: query
        name: name
        description: The domain namettttttttttttttexample
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:identifier:
    delete:
      summary: Delete an existing zone
      description: Delete an existing zone
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Zones
    get:
      summary: 'Zone details permission needed: #zone:read'
      description: 'Zone details permission needed: #zone:readntt'
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Zones
    patch:
      summary: Only one zone property can be changed at a time
      description: Only one zone property can be changed at a time
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-patch
      parameters:
      - in: query
        name: paused
        description: Indicates if the zone is only using CloudFlare DNS services
      - in: query
        name: plan
        description: The desired plan for the zone
      - in: query
        name: vanity_name_servers
        description: An array of domains used for custom name servers
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:identifier/activation_check:
    put:
      summary: 'Initiate another zone activation check permission needed: #zone:edit'
      description: 'Initiate another zone activation check permission needed: #zone:editntt'
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifieractivation-check-put
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:identifier/purge_cache:
    delete:
      summary: Remove ALL files from CloudFlare&#39;s cache
      description: Remove ALL files from CloudFlare&#39;s cache
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifierpurge-cache-delete
      parameters:
      - in: query
        name: files
        description: An array of URLs that should be removed from cachetttttttttttttt[http://www
      - in: query
        name: purge_everything
        description: A flag that indicates all resources in CloudFlares cache should
          be removed
      - in: query
        name: tags
        description: Any assets served with a Cache-Tag header that matches one of
          the provided values will be purged from the CloudFlare cachetttttttttttttt[some-tag,another-tag]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /user/billing/subscriptions/zones:
    get:
      summary: List all of your zone plan subscriptions
      description: List all of your zone plan subscriptions
      operationId: cloudflare-zone-subscription-api
      x-api-path-slug: userbillingsubscriptionszones-get
      parameters:
      - in: query
        name: activated_on
        description: When the subscription was activated2014-03-01T12:20:00Z
      - in: query
        name: cancelled_on
        description: When the subscription was cancelled2014-04-01T12:20:00Z
      - in: query
        name: direction
        description: Direction to order subscriptionsdesc
      - in: query
        name: expired_on
        description: When the subscription expired2014-04-02T12:20:00Z
      - in: query
        name: expires_on
        description: When the subscription will expire2014-03-31T12:20:00Z
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: order
        description: Field to order subscriptions bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of items per page20
      - in: query
        name: price
        description: The price of the subscription that will be billed, in US dollars20
      - in: query
        name: renewed_on
        description: When the subscription was renewed2014-05-11T12:20:00Z
      - in: query
        name: status
        description: The state of the subscriptionactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zone Subscriptions
  /user/billing/subscriptions/zones/:identifier:
    get:
      summary: Billing subscription details
      description: Billing subscription details
      operationId: cloudflare-zone-subscription-api
      x-api-path-slug: userbillingsubscriptionszonesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Zone Subscriptions