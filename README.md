# Reverse Engineering of Iceland Api


Iceland, online grocery delivery service


## Delivery States

### Out for delivery

This state is when a driver is 'out for delivery', this state is the first one i recorded.

```typescript
{
  result: string,                  // "OK"
  delivery_status: string,         // "Out for delivery"
  delivery_status_reason: string,  // ""
  estimated_delivery_time: string, // "13:46"
  internal_job_set_id: string,     // "20241027-1230-1430-DA67MUU-0578"
  delivery_slot_start: string,     // "13:30"
  delivery_slot_end: string,       // "14:30"
  delivery_completed: boolean,      // false
  delivery_date: string,           // "2024-10-27"
  delivery_time: string,           // "12:53:35"
  delivery_vehicle_reg: string,    // "DA67MUU"
  delivery_stop: number,           // 7.0
  drivers_name: string,            // "Anthony "
  jobs_attempted: number,          // 4
  map_image: string                 // "data:image/jpeg;base64,..."
}
```

#### Notables

internal_job_set_id is some form of internal database reference to the current delivery job, not certain why its being exposed on a public api. It follows a very clear pattern, `{delivery_date.replaceAll('-', '')}-{delivery_slot_start}-{delivery_slot_end}-{delivery_vehicle_reg}-{random 4 digits}`