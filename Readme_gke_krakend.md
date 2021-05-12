https://hackernoon.com/how-to-successfully-set-up-krakend-on-gke-a-step-by-step-guide-ny22311c

How to use GKE free tier


### 1. Create an external ip 

```
gcloud compute addresses create my-kraken-ip --global
gcloud compute addresses describe my-kraken-ip --global
gcloud compute addresses list
gcloud compute addresses delete my-kraken-ip --global
gcloud compute addresses list
```

### 2. Steup domain

//some.domain.dev
@               A           1h      <IP_ADDRESS_FROM_PREVIOUS_STEP>
kraken            CNAME       1h      cloud-mycomp.ca.

```
dig kraken.cloud-markham.ca
dig some.domain.io
```

### 3. Steup domain


```
gcloud domains verify cloud-markham.ca
dig cloud-markham.ca
dig bitwarden.cloud-markham.ca

```

