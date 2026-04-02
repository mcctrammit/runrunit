export default async function handler(req, res) {
  res.setHeader('Access-Control-Allow-Origin', '*');
  res.setHeader('Access-Control-Allow-Methods', 'GET, OPTIONS');
  res.setHeader('Access-Control-Allow-Headers', 'Content-Type');
  if (req.method === 'OPTIONS') return res.status(200).end();

  const RUNRUNIT_TOKEN  = process.env.RUNRUNIT_TOKEN;
  const RUNRUNIT_APPKEY = process.env.RUNRUNIT_APPKEY;

  try {
    const response = await fetch(
      'https://runrun.it/api/v1.0/tasks?limit=500&is_subtask=true&sort_by=updated_at&sort_order=desc',
      { headers: { 'App-Key': RUNRUNIT_APPKEY, 'User-Token': RUNRUNIT_TOKEN, 'Content-Type': 'application/json' } }
    );
    if (!response.ok) {
      const text = await response.text();
      return res.status(response.status).json({ error: text });
    }
    return res.status(200).json(await response.json());
  } catch (err) {
    return res.status(500).json({ error: err.message });
  }
}
